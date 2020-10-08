---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67d1d8efeb06c58d6628d0d7b922b3f16e8be1be
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374063"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTeam *team = [[MSGraphTeam alloc] init];
[team setDisplayName:@"My Class Team"];
[team setDescription:@"My Class Team’s Description"];
NSMutableArray *channelsList = [[NSMutableArray alloc] init];
MSGraphChannel *channels = [[MSGraphChannel alloc] init];
[channels setDisplayName:@"Class Announcements 📢"];
[channels setIsFavoriteByDefault: true];
[channelsList addObject: channels];
MSGraphChannel *channels = [[MSGraphChannel alloc] init];
[channels setDisplayName:@"Homework 🏋️"];
[channels setIsFavoriteByDefault: true];
[channelsList addObject: channels];
[team setChannels:channelsList];
MSGraphTeamMemberSettings *memberSettings = [[MSGraphTeamMemberSettings alloc] init];
[memberSettings setAllowCreateUpdateChannels: false];
[memberSettings setAllowDeleteChannels: false];
[memberSettings setAllowAddRemoveApps: false];
[memberSettings setAllowCreateUpdateRemoveTabs: false];
[memberSettings setAllowCreateUpdateRemoveConnectors: false];
[team setMemberSettings:memberSettings];
NSMutableArray *installedAppsList = [[NSMutableArray alloc] init];
MSGraphTeamsAppInstallation *installedApps = [[MSGraphTeamsAppInstallation alloc] init];
[installedAppsList addObject: installedApps];
MSGraphTeamsAppInstallation *installedApps = [[MSGraphTeamsAppInstallation alloc] init];
[installedAppsList addObject: installedApps];
[team setInstalledApps:installedAppsList];

NSError *error;
NSData *teamData = [team getSerializedDataWithError:&error];
[urlRequest setHTTPBody:teamData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```