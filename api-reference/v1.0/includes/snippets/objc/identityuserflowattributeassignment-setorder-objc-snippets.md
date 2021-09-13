---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef9f6f6ac7c8abc4c9d269b7dabf55ad0e2e8661326edd8f1da17a9ae25d96fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333153"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2xUserFlows/{id}/userAttributeAssignments/setOrder"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphAssignmentOrder *newAssignmentOrder = [[MSGraphAssignmentOrder alloc] init];
NSMutableArray *orderList = [[NSMutableArray alloc] init];
[orderList addObject: @"City"];
[orderList addObject: @"extension_GUID_ShoeSize"];
[newAssignmentOrder setOrder:orderList];
payloadDictionary[@"newAssignmentOrder"] = newAssignmentOrder;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```