---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c02c240caadfdbb8207b1db19f57461a5f189e9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338231"
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
targetedVariations.languageTag = "es-ES";
targetedVariations.displayName = "Sitio de instalación Contoso";
targetedVariations.description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto";
targetedVariationsList.add(targetedVariations);
bookmark.targetedVariations = targetedVariationsList;
LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupId");
bookmark.groupIds = groupIdsList;
LinkedList<String> powerAppIdsList = new LinkedList<String>();
powerAppIdsList.add("powerAppId");
bookmark.powerAppIds = powerAppIdsList;
bookmark.state = AnswerState.PUBLISHED;

graphClient.search().bookmarks()
    .buildRequest()
    .post(bookmark);

```