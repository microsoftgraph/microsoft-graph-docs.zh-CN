---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c29bef9d9e8f7012d46432ccfedec9d163e5af0
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791136"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/settings/regionalandlanguagesettings"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphRegionalAndLanguageSettings *regionalAndLanguageSettings = [[MSGraphRegionalAndLanguageSettings alloc] init];
MSGraphLocaleInfo *defaultDisplayLanguage = [[MSGraphLocaleInfo alloc] init];
[defaultDisplayLanguage setLocale:@"en-US"];
[regionalAndLanguageSettings setDefaultDisplayLanguage:defaultDisplayLanguage];
NSMutableArray *authoringLanguagesList = [[NSMutableArray alloc] init];
MSGraphLocaleInfo *authoringLanguages = [[MSGraphLocaleInfo alloc] init];
[authoringLanguages setLocale:@"fr-FR"];
[authoringLanguagesList addObject: authoringLanguages];
MSGraphLocaleInfo *authoringLanguages = [[MSGraphLocaleInfo alloc] init];
[authoringLanguages setLocale:@"de-DE"];
[authoringLanguagesList addObject: authoringLanguages];
[regionalAndLanguageSettings setAuthoringLanguages:authoringLanguagesList];
MSGraphLocaleInfo *defaultTranslationLanguage = [[MSGraphLocaleInfo alloc] init];
[defaultTranslationLanguage setLocale:@"en-US"];
[regionalAndLanguageSettings setDefaultTranslationLanguage:defaultTranslationLanguage];
MSGraphLocaleInfo *defaultSpeechInputLanguage = [[MSGraphLocaleInfo alloc] init];
[defaultSpeechInputLanguage setLocale:@"en-US"];
[regionalAndLanguageSettings setDefaultSpeechInputLanguage:defaultSpeechInputLanguage];
MSGraphLocaleInfo *defaultRegionalFormat = [[MSGraphLocaleInfo alloc] init];
[defaultRegionalFormat setLocale:@"en-GB"];
[regionalAndLanguageSettings setDefaultRegionalFormat:defaultRegionalFormat];
MSGraphRegionalFormatOverrides *regionalFormatOverrides = [[MSGraphRegionalFormatOverrides alloc] init];
[regionalFormatOverrides setCalendar:@"Gregorian Calendar"];
[regionalFormatOverrides setFirstDayOfWeek:@"Sunday"];
[regionalFormatOverrides setShortDateFormat:@"yyyy-MM-dd"];
[regionalFormatOverrides setLongDateFormat:@"dddd, MMMM d, yyyy"];
[regionalFormatOverrides setShortTimeFormat:@"HH:mm"];
[regionalFormatOverrides setLongTimeFormat:@"h:mm:ss tt"];
[regionalFormatOverrides setTimeZone:@"Pacific Standard Time"];
[regionalAndLanguageSettings setRegionalFormatOverrides:regionalFormatOverrides];

NSError *error;
NSData *regionalAndLanguageSettingsData = [regionalAndLanguageSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:regionalAndLanguageSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```