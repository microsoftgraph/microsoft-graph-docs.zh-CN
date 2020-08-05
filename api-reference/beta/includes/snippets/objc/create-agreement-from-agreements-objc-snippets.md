---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 204a1f557f76f4c4db927cc9a1256421f7753c92
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569907"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/agreements"]]];
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