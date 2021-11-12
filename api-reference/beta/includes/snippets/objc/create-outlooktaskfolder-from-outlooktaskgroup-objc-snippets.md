---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24f138cf20529309a2bc3aa6b8567f1f94359221032467a3beaf2aa5de510336
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106517"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTaskFolder *outlookTaskFolder = [[MSGraphOutlookTaskFolder alloc] init];
[outlookTaskFolder setName:@"Cooking"];

NSError *error;
NSData *outlookTaskFolderData = [outlookTaskFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookTaskFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```