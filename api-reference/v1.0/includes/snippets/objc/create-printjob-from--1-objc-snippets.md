---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 193c5570bcf339dbdbcf65284dae6846735867ca73c3b8552e29d9b85ba5006f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332242"
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