---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd3ddabbac6b01aa21a684c782d8d23ca908949a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719299"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Bookmark bookmark = new Bookmark();
bookmark.displayName = "Contoso Install Site";
bookmark.webUrl = "http://www.contoso.com/";
bookmark.description = "Try or buy Contoso for Home or Business and view product information";
AnswerKeyword keywords = new AnswerKeyword();
LinkedList<String> keywordsList = new LinkedList<String>();
keywordsList.add("Contoso");
keywordsList.add("install");
keywords.keywords = keywordsList;
LinkedList<String> reservedKeywordsList = new LinkedList<String>();
reservedKeywordsList.add("Contoso");
keywords.reservedKeywords = reservedKeywordsList;
keywords.matchSimilarKeywords = true;
bookmark.keywords = keywords;
bookmark.availabilityStartDateTime = OffsetDateTimeSerializer.deserialize("null");
bookmark.availabilityEndDateTime = OffsetDateTimeSerializer.deserialize("null");
LinkedList<DevicePlatformType> platformsList = new LinkedList<DevicePlatformType>();
platformsList.add(DevicePlatformType.ANDROID);
bookmark.platforms = platformsList;
LinkedList<AnswerVariant> targetedVariationsList = new LinkedList<AnswerVariant>();
AnswerVariant targetedVariations = new AnswerVariant();
targetedVariations.languageTag = "es-es";
targetedVariations.displayName = "Sitio de instalación Contoso";
targetedVariations.description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto";
targetedVariationsList.add(targetedVariations);
bookmark.targetedVariations = targetedVariationsList;
bookmark.state = AnswerState.PUBLISHED;

graphClient.search().bookmarks()
    .buildRequest()
    .post(bookmark);

```