---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 074a865ce3cc49019b64f5688f71267026011581118b9275dc9569efb38a9612
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237816"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookRangeFormat *workbookRangeFormat = [[MSGraphWorkbookRangeFormat alloc] init];
[workbookRangeFormat setColumnWidth: 135];
[workbookRangeFormat setHorizontalAlignment:@"Right"];
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