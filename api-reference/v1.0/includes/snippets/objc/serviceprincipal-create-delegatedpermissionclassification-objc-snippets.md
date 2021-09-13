---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0425c239d9278bdfda4ca597c93e8c078f5126eba455bb84939e626a25e1d836
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162351"
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