---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74102cd7e7456580fe20adee01d9f5cf4e0fad50
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338258"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Qna qna = new Qna();
qna.displayName = "Global Country Holidays";
qna.webUrl = "http://www.contoso.com/";
qna.description = "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend.    <table>    <thead>    <tr>    <td><strong>2021 Dates</strong></td>    <td><strong>Holiday</strong></td>    </tr>    </thead>    <tbody>    <tr>        <td>January 1, 2021</td>        <td>New Year's Day</td>    </tr>        <tr>        <td>January 18, 2021</td>        <td>Martin Luther King Day</td>    </tr>        <tr>        <td>February 15, 2021</td>        <td>Presidents Day</td>    </tr>        <tr>        <td>May 31, 2021</td>        <td>Memorial Day</td>    </tr>        <tr>        <td>July 5, 2021</td>        <td>Independence Day</td>    </tr>        <tr>        <td>September 6, 2021</td>        <td>Labor Day</td>    </tr>        <tr>        <td>November 25, 2021 - November 26, 2021</td>        <td>Thanksgiving Day and Day after Thanksgiving</td>    </tr>    <tr>        <td>December 23, 2021 - December 24, 2021</td>        <td>Christmas Eve and Christmas Day</td>    </tr>    </tbody>    </table>";
AnswerKeyword keywords = new AnswerKeyword();
LinkedList<String> keywordsList = new LinkedList<String>();
keywordsList.add("new years day");
keywordsList.add("martin luther king day");
keywordsList.add("presidents day");
keywordsList.add("memorial day");
keywordsList.add("independence day");
keywordsList.add("labor day");
keywordsList.add("thanksgiving");
keywordsList.add("christmas");
keywords.keywords = keywordsList;
LinkedList<String> reservedKeywordsList = new LinkedList<String>();
reservedKeywordsList.add("holidays");
reservedKeywordsList.add("paid days off");
keywords.reservedKeywords = reservedKeywordsList;
keywords.matchSimilarKeywords = true;
qna.keywords = keywords;
qna.availabilityStartDateTime = OffsetDateTimeSerializer.deserialize("2020-09-21T20:01:37Z");
qna.availabilityEndDateTime = OffsetDateTimeSerializer.deserialize("2021-12-31T20:01:37Z");
LinkedList<String> languageTagsList = new LinkedList<String>();
languageTagsList.add("en-US");
qna.languageTags = languageTagsList;
LinkedList<DevicePlatformType> platformsList = new LinkedList<DevicePlatformType>();
platformsList.add(DevicePlatformType.I_O_S);
qna.platforms = platformsList;
LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupId");
qna.groupIds = groupIdsList;
qna.state = AnswerState.PUBLISHED;

graphClient.search().qnas()
    .buildRequest()
    .post(qna);

```