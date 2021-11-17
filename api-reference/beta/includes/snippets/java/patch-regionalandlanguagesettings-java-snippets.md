---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a414672ec3cda6d47c5ba278d7e2145cf3e6a21075b49fe35d52d1f992210289
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RegionalAndLanguageSettings regionalAndLanguageSettings = new RegionalAndLanguageSettings();
LinkedList<LocaleInfo> authoringLanguagesList = new LinkedList<LocaleInfo>();
LocaleInfo authoringLanguages = new LocaleInfo();
authoringLanguages.locale = "en-US";
authoringLanguagesList.add(authoringLanguages);
LocaleInfo authoringLanguages1 = new LocaleInfo();
authoringLanguages1.locale = "es-MX";
authoringLanguagesList.add(authoringLanguages1);
regionalAndLanguageSettings.authoringLanguages = authoringLanguagesList;
LocaleInfo defaultRegionalFormat = new LocaleInfo();
defaultRegionalFormat.locale = "en-US";
regionalAndLanguageSettings.defaultRegionalFormat = defaultRegionalFormat;

graphClient.me().settings().regionalAndLanguageSettings()
    .buildRequest()
    .patch(regionalAndLanguageSettings);

```