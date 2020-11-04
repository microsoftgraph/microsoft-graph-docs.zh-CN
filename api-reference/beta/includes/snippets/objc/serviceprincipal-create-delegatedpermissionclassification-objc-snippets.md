---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77e92e0a70939a786902b009ee20eada18af8bc1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904788"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/delegatedPermissionClassifications"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDelegatedPermissionClassification *delegatedPermissionClassification = [[MSGraphDelegatedPermissionClassification alloc] init];
[delegatedPermissionClassification setPermissionId:@"e1fe6dd8-ba31-4d61-89e7-88639da4683d"];
[delegatedPermissionClassification setPermissionName:@"User.Read"];
[delegatedPermissionClassification setClassification: [MSGraphPermissionClassificationType low]];

NSError *error;
NSData *delegatedPermissionClassificationData = [delegatedPermissionClassification getSerializedDataWithError:&error];
[urlRequest setHTTPBody:delegatedPermissionClassificationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```