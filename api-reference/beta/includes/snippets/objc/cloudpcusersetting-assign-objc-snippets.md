---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42cdad4b59ba8f67276bc2e28cfd6f1f457684c15206016a40db11b7d301810e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162099"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *assignmentsList = [[NSMutableArray alloc] init];
MSGraphCloudPcUserSettingAssignment *assignments = [[MSGraphCloudPcUserSettingAssignment alloc] init];
[assignments setId:@"b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff"];
MSGraphCloudPcManagementAssignmentTarget *target = [[MSGraphCloudPcManagementAssignmentTarget alloc] init];
[target setGroupId:@"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"];
[assignments setTarget:target];
[assignmentsList addObject: assignments];
payloadDictionary[@"assignments"] = assignmentsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```