---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e210909147cb8fd5be4a46927bde56460f6763
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523094"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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