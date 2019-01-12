---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8febd66915ee0b4fba26d9253cd56d67086e63bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982895"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。

## <a name="properties"></a>属性

| 属性                           | 类型                          | 说明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | String                        | 可取值为：`default`、`voicemail`。 |
| identity                           | [identitySet](identityset.md) | 与此邀请关联[identitySet](identityset.md) 。                   |
| languageId                         | 字符串                        | 语言区域性字符串。                                                                                     |
| 区域                             | 字符串                        | 参与者的区域。                                                           |
| replacesCallId                     | 字符串                        | 可选。 呼叫的目标 idenity 目前的一部分。 一旦添加参与者，此呼叫将被丢弃。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
