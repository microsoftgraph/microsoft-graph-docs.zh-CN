---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9bfd8a3dec9b63972992210b064640f7d1df9136ca4504270d46cd5aaa88f8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279100"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskfolders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTaskFolder *outlookTaskFolder = [[MSGraphOutlookTaskFolder alloc] init];
[outlookTaskFolder setName:@"Volunteer"];

NSError *error;
NSData *outlookTaskFolderData = [outlookTaskFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookTaskFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```