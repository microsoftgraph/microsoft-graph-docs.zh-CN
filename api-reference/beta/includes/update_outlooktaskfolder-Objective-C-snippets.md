---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9943ee48ff9598917b91065bedd162cb276ea33c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330413"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTaskFolder *outlookTaskFolder = [[MSGraphOutlookTaskFolder alloc] init];
[outlookTaskFolder setName:@"Charity work"];

NSError *error;
NSData *outlookTaskFolderData = [outlookTaskFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookTaskFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```