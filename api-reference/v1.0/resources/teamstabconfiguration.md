---
title: teamsTabConfiguration 资源类型 (开放式类型)
description: 确定选项卡内容的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9873d9e03fec5d7751270b963015aed9eeb0ab48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456976"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>teamsTabConfiguration 资源类型 (开放式类型)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定[选项卡](teamstab.md)内容的设置。以交互方式配置选项卡时, 选项卡提供程序应用程序将设置此信息。
除了以下属性之外, 一些选项卡提供程序应用程序还指定其他自定义属性。

## <a name="properties"></a>属性

|属性|类型|说明|
|-|-|-|
|  entityId   |   字符串 |  由选项卡提供程序承载的实体的标识符。     |
|  contentUrl |   字符串 |  用于在团队中呈现选项卡内容的 Url。 必需。    |
|  removeUrl  |   字符串 |  使用团队客户端删除选项卡时, 由团队客户端调用的 Url。     |
|  websiteUrl |   string |  用于显示团队外部的选项卡内容的 Url。     |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstabconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
