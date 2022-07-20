---
title: 更新 learningContent
description: 更新 learningContent 对象的属性。
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 80e9caa91d973e90e0f7b8d9f4ccb07708dbdb4f
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883295"
---
# <a name="update-learningcontent"></a>更新 learningContent
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定的 [learningContent](../resources/learningcontent.md) 资源。 

[学习提供程序](../resources/learningprovider.md)用于在Viva Learning中引入或更新其内容的元数据。 如果指定的提供程序尚不存在指定的学习内容，则此操作将创建新内容的元数据。 否则，此操作将替换现有内容的元数据。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|LearningContent.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|LearningContent.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /employeeExperience/learningProviders/{registrationId}/learningContents(externalId='{externalId}') 
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|additionalTags|字符串集合|与学习内容关联的关键字、主题和其他标记。 可选。|
|contentWebUrl|String|学习内容的内容 Web URL。 必需。|
|贡献|String|学习内容的作者、创建者或参与者。 可选。|
|createdDateTime|DateTimeOffset|创建学习内容的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 可选。|
|说明|String|学习内容的说明或摘要。 可选。|
|duration|持续时间|学习内容的持续时间（以秒为单位）。 可选。|
|externalId|String|学习内容的唯一外部内容 ID。 必需。|
|format|String|学习内容的格式。 例如， ， `Course``Video`， `Book`， `Book Summary`。 `Audiobook Summary` 可选。|
|isActive|Boolean|指示内容是否处于活动状态。 非活动内容不会显示在 UI 中。 默认值为 `true`。 可选。|
|isPremium|布尔|指示学习内容是否要求用户在学习提供程序平台上登录。 默认值为 `false`。 可选。|
|isSearchable|布尔|指示学习内容是否可搜索。 默认值为 `true`。 可选。|
|languageTag|String|学习内容的语言，例如， `en-us` 或 `fr-fr`。 必需。|
|lastModifiedDateTime|DateTimeOffset|上次修改学习内容的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 可选。|
|numberOfPages|Int32|学习内容的页数，例如 9。 可选。|
|skillTags|字符串集合|与学习内容关联的技能标记。 可选。|
|sourceName|String|学习内容的源名称，例如 `LinkedIn Learning` 或 `Coursera`。 可选。|
|thumbnailWebUrl|String|学习内容缩略图图像的 URL。 可选。|
|title|String|学习内容的标题。 必需。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `202 Accepted` 响应代码和更新的 [learningContent](../resources/learningcontent.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "update_learningcontent"
}
-->
``` http
PATCH /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents(externalId='LP4471') 
Content-Type: application/json

{
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MsLearn",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 9,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningContent"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders('13727311-e7bb-470d-8b20-6a23d9030d70')/learningContents/$entity",
    "externalId": "LP4471",
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MsLearn",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 9,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```

