---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4a4d34e94fc54cd47ed6773e91c2fb62f0b62ce4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447708"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo 资源类型

命名空间： microsoft. graph

此资源用于表示受邀加入组呼叫的实体。 

## <a name="properties"></a>属性

| 属性                           | 类型                          | 说明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| 窃取                           | [identitySet](identityset.md) | 与此邀请关联的[了解 identityset](identityset.md) 。                   |
| replacesCallId                     | String                        | 可选。 目标标识当前是其一部分的调用。 添加参与者后，将删除此呼叫。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
