---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3abe47b7f3aa1acbd1193eed52f764021a5b0b841a1d0d1ade69eb78274c4ea2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378656"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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