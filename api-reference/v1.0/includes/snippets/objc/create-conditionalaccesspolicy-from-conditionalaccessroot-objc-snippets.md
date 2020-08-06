---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85a7e56791323b79ccc7c444ca445bbd533532aa
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565939"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/policies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConditionalAccessPolicy *conditionalAccessPolicy = [[MSGraphConditionalAccessPolicy alloc] init];
[conditionalAccessPolicy setDisplayName:@"Require MFA to EXO from non-compliant devices."];
[conditionalAccessPolicy setState: [MSGraphConditionalAccessPolicyState enabled]];
MSGraphConditionalAccessConditionSet *conditions = [[MSGraphConditionalAccessConditionSet alloc] init];
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
[conditionalAccessPolicy setConditions:conditions];
MSGraphConditionalAccessGrantControls *grantControls = [[MSGraphConditionalAccessGrantControls alloc] init];
[grantControls setOperator:@"OR"];
NSMutableArray *builtInControlsList = [[NSMutableArray alloc] init];
[builtInControlsList addObject: @"mfa"];
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