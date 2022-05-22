---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48928051447b295285062c0e05997515db78e7af
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629352"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/snapshots/getStorageAccounts(subscriptionId='cb6ad4c4-8a17-4245-a644-e4436b1ee204')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphCloudPcForensicStorageAccount *cloudPcForensicStorageAccount = [[MSGraphCloudPcForensicStorageAccount alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```