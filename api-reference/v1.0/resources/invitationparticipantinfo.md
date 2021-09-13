---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant** 用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f048fae8d5d63aac8a64dc0e8d3193de5cc5aef5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084424"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo 资源类型

命名空间：microsoft.graph

此资源用于表示受邀加入组呼叫的实体。 

## <a name="properties"></a>属性

| 属性                           | 类型                          | 说明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| identity                           | [identitySet](identityset.md) | 与此[邀请关联的 identitySet。](identityset.md)                   |
| replacesCallId                     | String                        | 可选。 目标标识当前属于的呼叫。 添加参与者后，将放弃此调用。 |

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

