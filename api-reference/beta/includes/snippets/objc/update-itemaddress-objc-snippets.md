---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c96852fe38ab57a3579e6bd9379739580681be62e4e8135a44e326970be389c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162799"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/addresses/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemAddress *itemAddress = [[MSGraphItemAddress alloc] init];
[itemAddress setAllowedAudiences: [MSGraphAllowedAudiences me]];
[itemAddress setDisplayName:@"Secret Hideout"];

NSError *error;
NSData *itemAddressData = [itemAddress getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemAddressData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```