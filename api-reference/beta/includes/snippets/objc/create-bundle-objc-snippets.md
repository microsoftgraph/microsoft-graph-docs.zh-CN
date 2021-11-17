---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c34873021d232f34432d4ed4a53b116e4e45c79fb5e05d0de12ec3dc658e2358
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105168"
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