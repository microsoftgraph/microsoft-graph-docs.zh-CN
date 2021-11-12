---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a1a4cc4a9eae2cc979110f4b37ca4c778d4ccaad7409ee7f6b1e4a82f278704
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277311"
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