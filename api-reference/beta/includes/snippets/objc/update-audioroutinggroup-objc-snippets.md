---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f58fad574922d11db0e07c5c21482d6367439fd805ed4f448527019a5a348116
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902897"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/{id}/audioRoutingGroups/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAudioRoutingGroup *audioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] init];
[audioRoutingGroup setId:@"oneToOne"];
[audioRoutingGroup setRoutingMode: [MSGraphRoutingMode oneToOne]];
NSMutableArray *sourcesList = [[NSMutableArray alloc] init];
[sourcesList addObject: @"632899f8-2ea1-4604-8413-27bd2892079f"];
[audioRoutingGroup setSources:sourcesList];
NSMutableArray *receiversList = [[NSMutableArray alloc] init];
[receiversList addObject: @"550fae72-d251-43ec-868c-373732c2704f"];
[receiversList addObject: @"72f988bf-86f1-41af-91ab-2d7cd011db47"];
[audioRoutingGroup setReceivers:receiversList];

NSError *error;
NSData *audioRoutingGroupData = [audioRoutingGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:audioRoutingGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```