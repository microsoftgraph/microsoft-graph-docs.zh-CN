---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48417e330ccc957dadc227975c829d360be05e4f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797452"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/policies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConditionalAccessPolicy *conditionalAccessPolicy = [[MSGraphConditionalAccessPolicy alloc] init];
[conditionalAccessPolicy setDisplayName:@"Require MFA to EXO from non-complaint devices."];
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
MSGraphConditionalAccessDevices *devices = [[MSGraphConditionalAccessDevices alloc] init];
NSMutableArray *includeDevicesList = [[NSMutableArray alloc] init];
[includeDevicesList addObject: @"All"];
[devices setIncludeDevices:includeDevicesList];
NSMutableArray *excludeDevicesList = [[NSMutableArray alloc] init];
[excludeDevicesList addObject: @"Compliant"];
[devices setExcludeDevices:excludeDevicesList];
[conditions setDevices:devices];
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