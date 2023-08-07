

# Extract NSP files from Fitgirl Repacks

This tool for Windows extracts Nintendo Switch game files (.NSP) from [Fitgirl Repacks](https://fitgirlrepacks.org/). 

You may want NSP files to play games on a modded Switch or emulator like Ryujinx.

### How to Use

- Download the latest `extractor.exe` from the [releases page](https://github.com/nytrancode/fitgirl-repack-nsp/releases).

- Copy `extractor.exe` into the Fitgirl Repack game folder (e.g. "C:/Games/Mario Kart 8 Deluxe"). 

- Double click `extractor.exe` to run it. The output file is `out.nsp` by default. 

- Or run from CMD/PowerShell to specify output filename:

```
extractor.exe -o mario-kart-8-deluxe.nsp
```

### How to Compile

- Requires Golang 1.16+

- Compile with:

```
GOOS=windows GOARCH=amd64 go build extractor.go
```

### Dependency 

- Uses [nspBuild](https://github.com/CVFireDragon/nspBuild/releases) by CVFireDragon
