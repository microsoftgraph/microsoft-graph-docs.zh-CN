---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf46f424389d1421b27ce49f976277b57d5aaf5c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956218"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/{printerId}/jobs"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrintJob *printJob = [[MSGraphPrintJob alloc] init];
MSGraphPrintJobConfiguration *configuration = [[MSGraphPrintJobConfiguration alloc] init];
[configuration setFeedOrientation: [MSGraphPrinterFeedOrientation longEdgeFirst]];
NSMutableArray *pageRangesList = [[NSMutableArray alloc] init];
MSGraphIntegerRange *pageRanges = [[MSGraphIntegerRange alloc] init];
[pageRanges setStart: 1];
[pageRanges setEnd: 1];
[pageRangesList addObject: pageRanges];
[configuration setPageRanges:pageRangesList];
[configuration setQuality: [MSGraphPrintQuality medium]];
[configuration setDpi: 600];
[configuration setOrientation: [MSGraphPrintOrientation landscape]];
[configuration setCopies: 1];
[configuration setDuplexMode: [MSGraphPrintDuplexMode oneSided]];
[configuration setColorMode: [MSGraphPrintColorMode blackAndWhite]];
[configuration setInputBin:@"by-pass-tray"];
[configuration setOutputBin:@"output-tray"];
[configuration setMediaSize:@"A4"];
MSGraphPrintMargin *margin = [[MSGraphPrintMargin alloc] init];
[margin setTop: 0];
[margin setBottom: 0];
[margin setLeft: 0];
[margin setRight: 0];
[configuration setMargin:margin];
[configuration setMediaType:@"stationery"];
[configuration setFinishings: null];
[configuration setPagesPerSheet: 1];
[configuration setMultipageLayout: [MSGraphPrintMultipageLayout clockwiseFromBottomLeft]];
[configuration setCollate: false];
[configuration setScaling: [MSGraphPrintScaling shrinkToFit]];
[configuration setFitPdfToPage: false];
[printJob setConfiguration:configuration];

NSError *error;
NSData *printJobData = [printJob getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printJobData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```