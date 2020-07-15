---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fb485a627ca88d0893586e8d08aa46aa55e657e
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142323"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"appplication/json" forHTTPHeaderField:@"Content-Type"];

MSGraphApplication *application = [[MSGraphApplication alloc] init];
MSGraphOnPremisesPublishing *onPremisesPublishing = [[MSGraphOnPremisesPublishing alloc] init];
MSGraphOnPremisesPublishingSingleSignOn *singleSignOnSettings = [[MSGraphOnPremisesPublishingSingleSignOn alloc] init];
MSGraphKerberosSignOnSettings *kerberosSignOnSettings = [[MSGraphKerberosSignOnSettings alloc] init];
[kerberosSignOnSettings setKerberosServicePrincipalName:@"HTTP/iwademo.contoso.com"];
[kerberosSignOnSettings setKerberosSignOnMappingAttributeType: [MSGraphKerberosSignOnMappingAttributeType userPrincipalName]];
[singleSignOnSettings setKerberosSignOnSettings:kerberosSignOnSettings];
[singleSignOnSettings setSingleSignOnMode: [MSGraphSingleSignOnMode onPremisesKerberos]];
[onPremisesPublishing setSingleSignOnSettings:singleSignOnSettings];
[application setOnPremisesPublishing:onPremisesPublishing];

NSError *error;
NSData *applicationData = [application getSerializedDataWithError:&error];
[urlRequest setHTTPBody:applicationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```