---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 135a5516806e5869aa9166f2fd6604fe0c374155ec9beeedcf36890f9f6d4e00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333318"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/skills/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSkillProficiency *skillProficiency = [[MSGraphSkillProficiency alloc] init];
NSMutableArray *categoriesList = [[NSMutableArray alloc] init];
[categoriesList addObject: @"Professional"];
[skillProficiency setCategories:categoriesList];
[skillProficiency setProficiency: [MSGraphSkillProficiencyLevel advancedProfessional]];

NSError *error;
NSData *skillProficiencyData = [skillProficiency getSerializedDataWithError:&error];
[urlRequest setHTTPBody:skillProficiencyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```