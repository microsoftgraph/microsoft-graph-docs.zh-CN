---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8227f27e58d142320c24a24884f1e4c2fdfdcc98
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920640"
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