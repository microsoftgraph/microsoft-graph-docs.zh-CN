---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 814f20c645211c0f7902640a461d5cfd2098c7f1361671e459185f0f1d019676
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105465"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphWorkbookRangeView *workbookRangeView = [[MSGraphWorkbookRangeView alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```