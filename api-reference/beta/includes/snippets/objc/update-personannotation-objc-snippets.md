---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 164cf9471ba2c8211bc7d57f9efa19bdde614adf0eba331dfb62d0810afc050d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220258"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/notes/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAnnotation *personAnnotation = [[MSGraphPersonAnnotation alloc] init];
[personAnnotation setAllowedAudiences: [MSGraphAllowedAudiences organization]];

NSError *error;
NSData *personAnnotationData = [personAnnotation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAnnotationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```