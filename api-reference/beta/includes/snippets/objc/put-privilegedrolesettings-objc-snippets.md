---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f4e86257ce1f4d8337d7e9713e3b4c06a37669b831151cf63c9e226b8fd6e6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220612"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoles/{id}/settings"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedRoleSettings *privilegedRoleSettings = [[MSGraphPrivilegedRoleSettings alloc] init];
[privilegedRoleSettings setId:@"9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3"];
[privilegedRoleSettings setElevationDuration:@"PT8H"];
[privilegedRoleSettings setNotificationToUserOnElevation: false];
[privilegedRoleSettings setTicketingInfoOnElevation: true];
[privilegedRoleSettings setMfaOnElevation: false];
[privilegedRoleSettings setMaxElavationDuration:@"PT0S"];
[privilegedRoleSettings setMinElevationDuration:@"PT0S"];
[privilegedRoleSettings setLastGlobalAdmin: false];
[privilegedRoleSettings setIsMfaOnElevationConfigurable: true];
[privilegedRoleSettings setApprovalOnElevation: false];
NSMutableArray *approverIdsList = [[NSMutableArray alloc] init];
[approverIdsList addObject: @"e2b2a2fb-13d7-495c-adc9-941fe966793f"];
[approverIdsList addObject: @"22770e3f-b9b4-418e-9dea-d0e3d2f275dd"];
[privilegedRoleSettings setApproverIds:approverIdsList];

NSError *error;
NSData *privilegedRoleSettingsData = [privilegedRoleSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedRoleSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```