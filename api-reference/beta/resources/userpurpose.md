---
title: userPurpose 资源类型
description: 代表 Exchange Online 中的用户的收件人或邮箱类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: b4ed5db9dfa87b2829d78371339c166c3bb74265
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846372"
---
# <a name="userpurpose-resource-type"></a>userPurpose 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

邮箱的用途。 用于将单个用户的邮箱与 Exchange Online 中的共享邮箱和设备邮箱区分开来。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---------------|:--------|:----------|
|值|[mailboxRecipientType](#mailboxrecipienttype-values)|代表 Exchange Online 中的用户的收件人或邮箱类型。 可能的值为：、、、、、 `unknown` `user` `linked` `shared` `room` `equipment` 和 `others` 。 有关详细信息，请参阅下一节。|

### <a name="mailboxrecipienttype-values"></a>mailboxRecipientType 值
|成员|说明|
|:---------------|:--------|
|unknown|找不到有关邮箱的任何信息。|
|用户|具有本地林中邮箱的用户帐户。|
|带有|链接到另一个林中的用户帐户的邮箱。|
|shared|由两个或更多用户帐户共享的邮箱。|
|室|表示会议室的邮箱。|
|器械|表示设备的邮箱。|
|一些|找到了邮箱，但用户目的与上面指定的不同。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userPurpose"
}-->

```json
{
    "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userPurpose resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
