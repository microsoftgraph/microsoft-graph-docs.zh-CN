---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ec82ca0805ffb5e6b07bf6a6e9bd38e91cf7bb5
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992709"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/11010/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/33223"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEducationSubmission *educationSubmission = [[MSGraphEducationSubmission alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```