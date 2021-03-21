---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abcb63a0c66d3b4a694a18d619367aff24968947
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982464"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
TranslationPreferences translationPreferences = new TranslationPreferences();
translationPreferences.translationBehavior = TranslationBehavior.YES;
LinkedList<TranslationLanguageOverride> languageOverridesList = new LinkedList<TranslationLanguageOverride>();
TranslationLanguageOverride languageOverrides = new TranslationLanguageOverride();
languageOverrides.languageTag = "fr";
languageOverrides.translationBehavior = TranslationBehavior.YES;
languageOverridesList.add(languageOverrides);
translationPreferences.languageOverrides = languageOverridesList;
regionalAndLanguageSettings.translationPreferences = translationPreferences;

graphClient.me().settings().regionalAndLanguageSettings()
    .buildRequest()
    .put(regionalAndLanguageSettings);

```