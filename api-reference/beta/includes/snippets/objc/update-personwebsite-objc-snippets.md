---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 373783dadae7bb3c93f926d4ae3daf440fcf5be522f9c953cbccc3fef31a3f38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215742"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/websites/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonWebsite *personWebsite = [[MSGraphPersonWebsite alloc] init];
[personWebsite setDescription:@"Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"];

NSError *error;
NSData *personWebsiteData = [personWebsite getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personWebsiteData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```