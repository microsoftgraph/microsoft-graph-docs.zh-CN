---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45d34555ce4e84e4a6b5e2ecf9c4780a6652032a4e8b195a53f92bce55cf0053
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104903"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/policies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConditionalAccessPolicy *conditionalAccessPolicy = [[MSGraphConditionalAccessPolicy alloc] init];
[conditionalAccessPolicy setDisplayName:@"Block access to EXO non-trusted regions."];
[conditionalAccessPolicy setState: [MSGraphConditionalAccessPolicyState enabled]];
MSGraphConditionalAccessConditionSet *conditions = [[MSGraphConditionalAccessConditionSet alloc] init];
NSMutableArray *clientAppTypesList = [[NSMutableArray alloc] init];
[clientAppTypesList addObject: @"all"];
[conditions setClientAppTypes:clientAppTypesList];
MSGraphConditionalAccessApplications *applications = [[MSGraphConditionalAccessApplications alloc] init];
NSMutableArray *includeApplicationsList = [[NSMutableArray alloc] init];
[includeApplicationsList addObject: @"00000002-0000-0ff1-ce00-000000000000"];
[applications setIncludeApplications:includeApplicationsList];
[conditions setApplications:applications];
MSGraphConditionalAccessUsers *users = [[MSGraphConditionalAccessUsers alloc] init];
NSMutableArray *includeGroupsList = [[NSMutableArray alloc] init];
[includeGroupsList addObject: @"ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"];
[users setIncludeGroups:includeGroupsList];
[conditions setUsers:users];
MSGraphConditionalAccessLocations *locations = [[MSGraphConditionalAccessLocations alloc] init];
NSMutableArray *includeLocationsList = [[NSMutableArray alloc] init];
[includeLocationsList addObject: @"198ad66e-87b3-4157-85a3-8a7b51794ee9"];
[locations setIncludeLocations:includeLocationsList];
[conditions setLocations:locations];
[conditionalAccessPolicy setConditions:conditions];
MSGraphConditionalAccessGrantControls *grantControls = [[MSGraphConditionalAccessGrantControls alloc] init];
[grantControls setOperator:@"OR"];
NSMutableArray *builtInControlsList = [[NSMutableArray alloc] init];
[builtInControlsList addObject: @"block"];
[grantControls setBuiltInControls:builtInControlsList];
[conditionalAccessPolicy setGrantControls:grantControls];

NSError *error;
NSData *conditionalAccessPolicyData = [conditionalAccessPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:conditionalAccessPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```