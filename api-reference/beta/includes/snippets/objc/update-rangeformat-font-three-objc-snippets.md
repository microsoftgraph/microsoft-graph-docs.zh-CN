---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c68ab1c123ace1ea07d5cdb0c536018e05fa6bb3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727947"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFont *workbookRangeFont = [[MSGraphWorkbookRangeFont alloc] init];
[workbookRangeFont setUnderline:@"Single"];
[workbookRangeFont setColor:@"#FFFFFF"];
[workbookRangeFont setSize: 26];

NSError *error;
NSData *workbookRangeFontData = [workbookRangeFont getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookRangeFontData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```