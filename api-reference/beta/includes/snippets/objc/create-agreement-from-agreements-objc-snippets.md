---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9c5f20bc6346b2bc039edd9ea761a46778306d10137dd65df9a9f8dcfe71d8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902537"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/termsOfUse/agreements"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAgreement *agreement = [[MSGraphAgreement alloc] init];
[agreement setDisplayName:@"MSGraph Sample"];
[agreement setIsViewingBeforeAcceptanceRequired: true];
NSMutableArray *filesList = [[NSMutableArray alloc] init];
MSGraphAgreementFileLocalization *files = [[MSGraphAgreementFileLocalization alloc] init];
[files setFileName:@"TOU.pdf"];
[files setLanguage:@"en"];
[files setIsDefault: true];
MSGraphAgreementFileData *fileData = [[MSGraphAgreementFileData alloc] init];
[fileData setData:@"SGVsbG8gd29ybGQ="];
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