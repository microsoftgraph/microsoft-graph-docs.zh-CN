---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a932f6c73bd0d57f1613ddced95606ba7d85046b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863558"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/timeOffRequests"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *timeOffRequestList = [[NSMutableArray alloc] init];
        timeOffRequestList = [jsonFinal valueForKey:@"value"];
        MSGraphTimeOffRequest *timeOffRequest = [[MSGraphTimeOffRequest alloc] initWithDictionary:[timeOffRequestList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```