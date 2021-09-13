---
title: 位置资源类型
description: 表示事件的位置信息。
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 678550a8683bf965dbc231055b60bd8a5b95c3df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134715"
---
# <a name="location-resource-type"></a>位置资源类型

命名空间：microsoft.graph

表示[事件](event.md)的位置信息。

可采用多种方法在日历中创建事件，例如，通过应用使用 [create event](../api/user-post-events.md) REST API，或者手动使用 Outlook 用户界面。 在使用用户界面创建事件时，可以以纯文本格式（例如，“Harry's Bar”）指定位置，或者从 Outlook 提供的会议室列表、[必应自动建议](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)或[必应本地搜索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)中指定位置。 

根据事件的创建方式，Outlook 应以不同方式设置只读 **locationType** 属性。 

| 事件的创建方式  | 属性   | 预期值 |
|:----------|:-------|:--------------------------------|
| [create event](../api/user-post-events.md) REST API | **locationType** | `default` |
| Outlook 中的用户界面 | **locationType** | 以下各项之一： <ul><li>`default`，以纯文本格式输入的位置。</li><li>`conferenceRoom`，Outlook 会议室列表提供的会议室。</li><li>或者，该列表中的任意项：`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress`，必应自动建议或必应本地搜索中的位置。</li></ul> |

## <a name="properties"></a>属性
| 属性  | 类型   | 说明                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicaladdress.md) |位置的街道地址。 |
| coordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 地理坐标和位置的海拔高度。 |
| displayName  | String | 与地点相关联的名称。                       |
| locationEmailAddress | String | （可选）与位置相关联的电子邮件地址。              |
| locationUri | String | （可选）表示位置的 URI。 |
| locationType | locationType | 位置的类型。 可能的值包括 `default` `conferenceRoom` `homeAddress` `businessAddress` `geoCoordinates` `streetAddress` ：、、、。 `hotel` `restaurant` `localBusiness` `postalAddress` 只读。|
| uniqueId | String | 仅供内部使用。|
| uniqueIdType | locationUniqueIdType | 仅供内部使用。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

