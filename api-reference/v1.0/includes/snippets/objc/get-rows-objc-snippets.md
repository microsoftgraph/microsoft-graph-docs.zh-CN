---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec66c50bf7daed7492dcbcd5038c30b81809e0e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492872"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *workbookRangeViewList = [[NSMutableArray alloc] init];
        workbookRangeViewList = [jsonFinal valueForKey:@"value"];
        MSGraphWorkbookRangeView *workbookRangeView = [[MSGraphWorkbookRangeView alloc] initWithDictionary:[workbookRangeViewList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```