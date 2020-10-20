---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 810a7e3b8f243ec631a497445841ec2d492afc53
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618967"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFormat *workbookRangeFormat = [[MSGraphWorkbookRangeFormat alloc] init];
[workbookRangeFormat setColumnWidth: 135];
[workbookRangeFormat setVerticalAlignment:@"Top"];
[workbookRangeFormat setRowHeight: 49];
[workbookRangeFormat setWrapText: false];

NSError *error;
NSData *workbookRangeFormatData = [workbookRangeFormat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookRangeFormatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```