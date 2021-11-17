---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13f1ab8a06b42eaac83dd07ed8c54dc6ec135679f7935ca8053679d60fac9c65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221294"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/projects"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProjectParticipation *projectParticipation = [[MSGraphProjectParticipation alloc] init];
NSMutableArray *categoriesList = [[NSMutableArray alloc] init];
[categoriesList addObject: @"Branding"];
[projectParticipation setCategories:categoriesList];
MSGraphCompanyDetail *client = [[MSGraphCompanyDetail alloc] init];
[client setDisplayName:@"Contoso Ltd."];
[client setDepartment:@"Corporate Marketing"];
[client setWebUrl:@"https://www.contoso.com"];
[projectParticipation setClient:client];
[projectParticipation setDisplayName:@"Contoso Re-branding Project"];
MSGraphPositionDetail *detail = [[MSGraphPositionDetail alloc] init];
MSGraphCompanyDetail *company = [[MSGraphCompanyDetail alloc] init];
[company setDisplayName:@"Adventureworks Inc."];
[company setDepartment:@"Consulting"];
[company setWebUrl:@"https://adventureworks.com"];
[detail setCompany:company];
[detail setDescription:@"Rebranding of Contoso Ltd."];
[detail setJobTitle:@"Lead PM Rebranding"];
[detail setRole:@"project management"];
[detail setSummary:@"A 6 month project to help Contoso rebrand after they were divested from a parent organization."];
[projectParticipation setDetail:detail];

NSError *error;
NSData *projectParticipationData = [projectParticipation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:projectParticipationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```