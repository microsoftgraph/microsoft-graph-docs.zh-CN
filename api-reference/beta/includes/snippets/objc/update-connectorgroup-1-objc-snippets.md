---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbcef68bc1e4a63dd38d261dd42a0da6a27f440a4bb30e42b4698f36f2656907
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158307"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/applicationProxy/connectorGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConnectorGroup *connectorGroup = [[MSGraphConnectorGroup alloc] init];
[connectorGroup setName:@"Connector Group Demo"];

NSError *error;
NSData *connectorGroupData = [connectorGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectorGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```