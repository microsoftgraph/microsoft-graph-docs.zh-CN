---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c0292adf00f7b50e99275ec729802695eae9e79d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323131"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id|userPrincipalName}/photo"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProfilePhoto *profilePhoto = [[MSGraphProfilePhoto alloc] init];
[profilePhoto setHeight: 99];
[profilePhoto setWidth: 99];
[profilePhoto setId:@"id-value"];

NSError *error;
NSData *profilePhotoData = [profilePhoto getSerializedDataWithError:&error];
[urlRequest setHTTPBody:profilePhotoData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```