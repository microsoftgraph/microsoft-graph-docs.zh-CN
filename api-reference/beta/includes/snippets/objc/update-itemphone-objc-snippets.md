---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bcf5ab38acfeb0c1e5e81e575226f402db3eb610382d886c1b0136a614b1961
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105142"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/phones/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPhone *itemPhone = [[MSGraphItemPhone alloc] init];
[itemPhone setType: [MSGraphPhoneType other]];

NSError *error;
NSData *itemPhoneData = [itemPhone getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPhoneData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```