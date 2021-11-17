---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f3070f7f2a7916e7f04402f8dc5adfb25c69dfc895034172aa1e89f7ba4407b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328743"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/settings/regionalandlanguagesettings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphRegionalAndLanguageSettings *regionalAndLanguageSettings = [[MSGraphRegionalAndLanguageSettings alloc] init];
NSMutableArray *authoringLanguagesList = [[NSMutableArray alloc] init];
MSGraphLocaleInfo *authoringLanguages = [[MSGraphLocaleInfo alloc] init];
[authoringLanguages setLocale:@"en-US"];
[authoringLanguagesList addObject: authoringLanguages];
MSGraphLocaleInfo *authoringLanguages = [[MSGraphLocaleInfo alloc] init];
[authoringLanguages setLocale:@"es-MX"];
[authoringLanguagesList addObject: authoringLanguages];
[regionalAndLanguageSettings setAuthoringLanguages:authoringLanguagesList];
MSGraphLocaleInfo *defaultRegionalFormat = [[MSGraphLocaleInfo alloc] init];
[defaultRegionalFormat setLocale:@"en-US"];
[regionalAndLanguageSettings setDefaultRegionalFormat:defaultRegionalFormat];

NSError *error;
NSData *regionalAndLanguageSettingsData = [regionalAndLanguageSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:regionalAndLanguageSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```