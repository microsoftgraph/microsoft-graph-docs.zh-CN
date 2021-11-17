---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bdd6be0a239efb7e9e9875529feeedd972015d7a31be78b0a4f337508d3495a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163786"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/skills"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSkillProficiency *skillProficiency = [[MSGraphSkillProficiency alloc] init];
NSMutableArray *categoriesList = [[NSMutableArray alloc] init];
[categoriesList addObject: @"Professional"];
[skillProficiency setCategories:categoriesList];
[skillProficiency setAllowedAudiences: [MSGraphAllowedAudiences organization]];
[skillProficiency setDisplayName:@"API Design"];
[skillProficiency setProficiency: [MSGraphSkillProficiencyLevel generalProfessional]];
NSMutableArray *collaborationTagsList = [[NSMutableArray alloc] init];
[collaborationTagsList addObject: @"ableToMentor"];
[skillProficiency setCollaborationTags:collaborationTagsList];

NSError *error;
NSData *skillProficiencyData = [skillProficiency getSerializedDataWithError:&error];
[urlRequest setHTTPBody:skillProficiencyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```