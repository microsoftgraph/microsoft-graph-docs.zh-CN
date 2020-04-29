---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f53777be8582d805f2a5aef98ca9e1853ad4cbc0
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43935156"
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
NSMutableArray *includeDeviceStatesList = [[NSMutableArray alloc] init];
[includeDeviceStatesList addObject: @"All"];
[devices setIncludeDeviceStates:includeDeviceStatesList];
NSMutableArray *excludeDeviceStatesList = [[NSMutableArray alloc] init];
[excludeDeviceStatesList addObject: @"Compliant"];
[devices setExcludeDeviceStates:excludeDeviceStatesList];
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