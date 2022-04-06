---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c1153dacfb883a576fa9160fbd225e71639e7ec
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528170"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/termsOfUse/agreements"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAgreement *agreement = [[MSGraphAgreement alloc] init];
[agreement setDisplayName:@"Contoso ToU for guest users"];
[agreement setIsViewingBeforeAcceptanceRequired: true];
NSMutableArray *filesList = [[NSMutableArray alloc] init];
MSGraphAgreementFileLocalization *files = [[MSGraphAgreementFileLocalization alloc] init];
[files setFileName:@"TOU.pdf"];
[files setLanguage:@"en"];
[files setIsDefault: true];
MSGraphAgreementFileData *fileData = [[MSGraphAgreementFileData alloc] init];
[fileData setData:@"SGVsbG8gd29ybGQ=//truncated-binary"];
[files setFileData:fileData];
[filesList addObject: files];
[agreement setFiles:filesList];

NSError *error;
NSData *agreementData = [agreement getSerializedDataWithError:&error];
[urlRequest setHTTPBody:agreementData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```