---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47cc7c6da8c1ee1a3536149a3d3c713ae2f316da
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843583"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphPrintJobConfiguration *printJobConfiguration = [[MSGraphPrintJobConfiguration alloc] init];
[printJobConfiguration setFeedOrientation: [MSGraphPrinterFeedOrientation longEdgeFirst]];
NSMutableArray *pageRangesList = [[NSMutableArray alloc] init];
MSGraphIntegerRange *pageRanges = [[MSGraphIntegerRange alloc] init];
[pageRanges setStart: 1];
[pageRanges setEnd: 1];
[pageRangesList addObject: pageRanges];
[printJobConfiguration setPageRanges:pageRangesList];
[printJobConfiguration setQuality: [MSGraphPrintQuality medium]];
[printJobConfiguration setDpi: 600];
[printJobConfiguration setOrientation: [MSGraphPrintOrientation landscape]];
[printJobConfiguration setCopies: 1];
[printJobConfiguration setDuplexMode: [MSGraphPrintDuplexMode oneSided]];
[printJobConfiguration setColorMode: [MSGraphPrintColorMode blackAndWhite]];
[printJobConfiguration setInputBin:@"by-pass-tray"];
[printJobConfiguration setOutputBin:@"output-tray"];
[printJobConfiguration setMediaSize:@"A4"];
MSGraphPrintMargin *margin = [[MSGraphPrintMargin alloc] init];
[margin setTop: 0];
[margin setBottom: 0];
[margin setLeft: 0];
[margin setRight: 0];
[printJobConfiguration setMargin:margin];
[printJobConfiguration setMediaType:@"stationery"];
[printJobConfiguration setFinishings: null];
[printJobConfiguration setPagesPerSheet: 1];
[printJobConfiguration setMultipageLayout: [MSGraphPrintMultipageLayout clockwiseFromBottomLeft]];
[printJobConfiguration setCollate: false];
[printJobConfiguration setScaling: [MSGraphPrintScaling shrinkToFit]];
[printJobConfiguration setFitPdfToPage: false];

NSError *error;
NSData *printJobConfigurationData = [printJobConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printJobConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```