---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a63d6597e7701985b468ff2f1fe055846f6f0ef
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709986"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls/{id}/audioRoutingGroups/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAudioRoutingGroup *AudioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] init];
[AudioRoutingGroup setId:@"oneToOne"];
[AudioRoutingGroup setRoutingMode: [MSGraphRoutingMode OneToOne]];
NSMutableArray *sourcesList = [[NSMutableArray alloc] init];
[sourcesList addObject: @"632899f8-2ea1-4604-8413-27bd2892079f"];
[AudioRoutingGroup setSources:sourcesList];
NSMutableArray *receiversList = [[NSMutableArray alloc] init];
[receiversList addObject: @"550fae72-d251-43ec-868c-373732c2704f"];
[receiversList addObject: @"72f988bf-86f1-41af-91ab-2d7cd011db47"];
[AudioRoutingGroup setReceivers:receiversList];

NSError *error;
NSData *AudioRoutingGroupData = [AudioRoutingGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:AudioRoutingGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```