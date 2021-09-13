---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16fdd2deb61e2c1ef74e75ddaf98cade9276010421c6854217a4281c9aa1452b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161803"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFormat *workbookRangeFormat = [[MSGraphWorkbookRangeFormat alloc] init];
[workbookRangeFormat setColumnWidth: 135];
[workbookRangeFormat setHorizontalAlignment:@"Center"];
[workbookRangeFormat setVerticalAlignment:@"Center"];
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