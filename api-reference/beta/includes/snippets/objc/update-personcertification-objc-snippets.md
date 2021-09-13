---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 454ed804803fed0d2790fc07d4e1afb3079983cbd64be9e21104562fccf9ef60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162772"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/certifications/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonCertification *personCertification = [[MSGraphPersonCertification alloc] init];
[personCertification setIssuingAuthority:@"International Academy of Marketing Excellence"];
[personCertification setIssuingCompany:@"International Academy of Marketing Excellence"];

NSError *error;
NSData *personCertificationData = [personCertification getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personCertificationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```