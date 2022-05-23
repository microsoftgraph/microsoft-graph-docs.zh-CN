---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cad401e88317a5fa3c327ce4ce65340f7ec9ade
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629236"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/files"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAgreementFileLocalization *agreementFileLocalization = [[MSGraphAgreementFileLocalization alloc] init];
[agreementFileLocalization setFileName:@"Contoso ToU for guest users (French)"];
[agreementFileLocalization setLanguage:@"fr-FR"];
[agreementFileLocalization setIsDefault: false];
[agreementFileLocalization setIsMajorVersion: false];
[agreementFileLocalization setDisplayName:@"Contoso ToU for guest users (French)"];
MSGraphAgreementFileData *fileData = [[MSGraphAgreementFileData alloc] init];
[fileData setData:@"base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data"];
[agreementFileLocalization setFileData:fileData];

NSError *error;
NSData *agreementFileLocalizationData = [agreementFileLocalization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:agreementFileLocalizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```