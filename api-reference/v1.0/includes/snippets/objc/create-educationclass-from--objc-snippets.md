---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b04753558106fc21ae66fa4edb85848a9d946941ff7048260015c55a1c33e34f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104994"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationClass *educationClass = [[MSGraphEducationClass alloc] init];
[educationClass setDisplayName:@"String"];
[educationClass setMailNickname:@"String"];
[educationClass setDescription:@"String"];
MSGraphIdentitySet *createdBy = [[MSGraphIdentitySet alloc] init];
[educationClass setCreatedBy:createdBy];
[educationClass setClassCode:@"String"];
[educationClass setExternalName:@"String"];
[educationClass setExternalId:@"String"];
[educationClass setExternalSource: [MSGraphEducationExternalSource sis]];
[educationClass setExternalSourceDetail:@"String"];
[educationClass setGrade:@"String"];
MSGraphEducationTerm *term = [[MSGraphEducationTerm alloc] init];
[educationClass setTerm:term];

NSError *error;
NSData *educationClassData = [educationClass getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationClassData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```