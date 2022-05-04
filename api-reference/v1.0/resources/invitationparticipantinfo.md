---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant** 用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c09e15063524fbba0f9a53b69786545399c8e35a
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191680"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo 资源类型

命名空间：microsoft.graph

此资源用于表示受邀进行组调用的实体。 

## <a name="properties"></a>属性

| 属性                           | 类型                          | 说明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| 身份                           | [identitySet](identityset.md) | 与此邀请关联的 [identitySet](identityset.md) 。                   |
| participantId                      | String                        | 可选。 目标参与者的 ID。                                          |
| replacesCallId                     | String                        | 可选。 目标标识当前所属的调用。 对于对等情况，一旦成功添加参与者，将放弃调用。 |

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
  "participantId": "String",  
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

