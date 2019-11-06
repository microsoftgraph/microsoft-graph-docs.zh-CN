---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 938e98673012d3f6ddf26325babd2fcea7851367
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997324"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/phones/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPhone *itemPhone = [[MSGraphItemPhone alloc] init];
[itemPhone setDisplayName:@"displayName-value"];
[itemPhone setType: [MSGraphPhoneType home]];
[itemPhone setNumber:@"number-value"];

NSError *error;
NSData *itemPhoneData = [itemPhone getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPhoneData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```