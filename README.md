# List-GitHubAssembly

Fetch a list of avaialble artifacts from the configured GitHub repo. 

# Execute-GitHubAssembly

Download the specified artifact and execute using Execute-Assembly.

Depends on a Github Actions workflow which outputs .NET assemblies compatible with Execute-Assembly. 

## Known Issues

This code depends on downloading artifacts from GitHub to the CS team server. You may run into an issue where the assembly inslt fully downloaded, or extracted, before Execute-Assembly is called. 

The sleep() call on line 55 and the while loop on line 198 can be adjusted to compensatefor slower network connectins. Some experimentatino may be required. 

## Credits

Some code from [SharpCompile](https://github.com/SpiderLabs/SharpCompile/blob/master/SharpCompile.cna) and [Beaconpire](https://github.com/bluscreenofjeff/AggressorScripts/blob/master/Beaconpire/beaconpire.cna) was adapted for this project. 

