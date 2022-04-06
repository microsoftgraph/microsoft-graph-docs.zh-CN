---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb771961327dfc3c130898a1f62c444761313a4f
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757703"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/bundles"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDriveItem *driveItem = [[MSGraphDriveItem alloc] init];
[driveItem setName:@"Just some files"];
[driveItem set@microsoft.graph.conflictBehavior:@"rename"];
MSGraphBundle *bundle = [[MSGraphBundle alloc] init];
[driveItem setBundle:bundle];
NSMutableArray *childrenList = [[NSMutableArray alloc] init];
MSGraphDriveItem *children = [[MSGraphDriveItem alloc] init];
[children setId:@"1234asdf"];
[childrenList addObject: children];
MSGraphDriveItem *children = [[MSGraphDriveItem alloc] init];
[children setId:@"1234qwerty"];
[childrenList addObject: children];
[driveItem setChildren:childrenList];

NSError *error;
NSData *driveItemData = [driveItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:driveItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```