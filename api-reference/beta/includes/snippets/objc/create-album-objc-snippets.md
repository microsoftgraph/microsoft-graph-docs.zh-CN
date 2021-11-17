---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d2ba7c4fda2ae5caba16587789d130942ace356bdcac1586afef602e64760ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105173"
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