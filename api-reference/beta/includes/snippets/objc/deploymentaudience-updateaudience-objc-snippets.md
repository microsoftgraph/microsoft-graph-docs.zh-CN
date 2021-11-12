---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcf270c614a353e0af0b632bb2ee038135623e519b859272712b458127a129c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333682"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *addMembersList = [[NSMutableArray alloc] init];
MSGraphWindowsUpdatesUpdatableAsset *addMembers = [[MSGraphWindowsUpdatesUpdatableAsset alloc] init];
[addMembers setId:@"String (identifier)"];
[addMembersList addObject: addMembers];
payloadDictionary[@"addMembers"] = addMembersList;

NSMutableArray *removeMembersList = [[NSMutableArray alloc] init];
MSGraphWindowsUpdatesUpdatableAsset *removeMembers = [[MSGraphWindowsUpdatesUpdatableAsset alloc] init];
[removeMembers setId:@"String (identifier)"];
[removeMembersList addObject: removeMembers];
payloadDictionary[@"removeMembers"] = removeMembersList;

NSMutableArray *addExclusionsList = [[NSMutableArray alloc] init];
MSGraphWindowsUpdatesUpdatableAsset *addExclusions = [[MSGraphWindowsUpdatesUpdatableAsset alloc] init];
[addExclusions setId:@"String (identifier)"];
[addExclusionsList addObject: addExclusions];
payloadDictionary[@"addExclusions"] = addExclusionsList;

NSMutableArray *removeExclusionsList = [[NSMutableArray alloc] init];
MSGraphWindowsUpdatesUpdatableAsset *removeExclusions = [[MSGraphWindowsUpdatesUpdatableAsset alloc] init];
[removeExclusions setId:@"String (identifier)"];
[removeExclusionsList addObject: removeExclusions];
payloadDictionary[@"removeExclusions"] = removeExclusionsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```