---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 704e1a3d46b58fb1aaef41cce5e28d85c65dafdf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997760"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/skills"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSkillProficiency *skillProficiency = [[MSGraphSkillProficiency alloc] init];
NSMutableArray *categoriesList = [[NSMutableArray alloc] init];
[categoriesList addObject: @"categories-value"];
[skillProficiency setCategories:categoriesList];
[skillProficiency setDisplayName:@"displayName-value"];
[skillProficiency setProficiency: [MSGraphSkillProficiencyLevel elementary]];
[skillProficiency setWebUrl:@"webUrl-value"];

NSError *error;
NSData *skillProficiencyData = [skillProficiency getSerializedDataWithError:&error];
[urlRequest setHTTPBody:skillProficiencyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```