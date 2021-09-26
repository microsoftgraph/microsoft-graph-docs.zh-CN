---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63ecb2c6e0ca14b24e828b0c5ac61d7ea3791e3d0146a7ae83017bbd6f5a1a24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277439"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroup *group = [[MSGraphGroup alloc] init];
NSMutableArray *assignedLabelsList = [[NSMutableArray alloc] init];
MSGraphAssignedLabel *assignedLabels = [[MSGraphAssignedLabel alloc] init];
[assignedLabels setLabelId:@"45cd0c48-c540-4358-ad79-a3658cdc5b88"];
[assignedLabelsList addObject: assignedLabels];
[group setAssignedLabels:assignedLabelsList];

NSError *error;
NSData *groupData = [group getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```