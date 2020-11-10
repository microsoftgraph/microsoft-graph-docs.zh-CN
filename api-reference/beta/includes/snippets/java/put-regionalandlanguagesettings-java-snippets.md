---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42c56e9db9c72310d8de905847232bd6658d80d6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966827"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RegionalAndLanguageSettings regionalAndLanguageSettings = new RegionalAndLanguageSettings();
LocaleInfo defaultDisplayLanguage = new LocaleInfo();
defaultDisplayLanguage.locale = "en-US";
regionalAndLanguageSettings.defaultDisplayLanguage = defaultDisplayLanguage;
LinkedList<LocaleInfo> authoringLanguagesList = new LinkedList<LocaleInfo>();
LocaleInfo authoringLanguages = new LocaleInfo();
authoringLanguages.locale = "fr-FR";
authoringLanguagesList.add(authoringLanguages);
LocaleInfo authoringLanguages1 = new LocaleInfo();
authoringLanguages1.locale = "de-DE";
authoringLanguagesList.add(authoringLanguages1);
regionalAndLanguageSettings.authoringLanguages = authoringLanguagesList;
LocaleInfo defaultTranslationLanguage = new LocaleInfo();
defaultTranslationLanguage.locale = "en-US";
regionalAndLanguageSettings.defaultTranslationLanguage = defaultTranslationLanguage;
LocaleInfo defaultSpeechInputLanguage = new LocaleInfo();
defaultSpeechInputLanguage.locale = "en-US";
regionalAndLanguageSettings.defaultSpeechInputLanguage = defaultSpeechInputLanguage;
LocaleInfo defaultRegionalFormat = new LocaleInfo();
defaultRegionalFormat.locale = "en-GB";
regionalAndLanguageSettings.defaultRegionalFormat = defaultRegionalFormat;
RegionalFormatOverrides regionalFormatOverrides = new RegionalFormatOverrides();
regionalFormatOverrides.calendar = "Gregorian Calendar";
regionalFormatOverrides.firstDayOfWeek = "Sunday";
regionalFormatOverrides.shortDateFormat = "yyyy-MM-dd";
regionalFormatOverrides.longDateFormat = "dddd, MMMM d, yyyy";
regionalFormatOverrides.shortTimeFormat = "HH:mm";
regionalFormatOverrides.longTimeFormat = "h:mm:ss tt";
regionalFormatOverrides.timeZone = "Pacific Standard Time";
regionalAndLanguageSettings.regionalFormatOverrides = regionalFormatOverrides;

graphClient.me().settings().regionalAndLanguageSettings()
    .buildRequest()
    .put(regionalAndLanguageSettings);

```