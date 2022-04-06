---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c2138eaf656472c1a6395902a5bb3da18c52175
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757702"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/bundles"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDriveItem *driveItem = [[MSGraphDriveItem alloc] init];
[driveItem setName:@"My Day at the Beach"];
[driveItem set@microsoft.graph.conflictBehavior:@"rename"];
MSGraphBundle *bundle = [[MSGraphBundle alloc] init];
MSGraphAlbum *album = [[MSGraphAlbum alloc] init];
[bundle setAlbum:album];
[driveItem setBundle:bundle];
NSMutableArray *childrenList = [[NSMutableArray alloc] init];
MSGraphDriveItem *children = [[MSGraphDriveItem alloc] init];
[children setId:@"1234asdf"];
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