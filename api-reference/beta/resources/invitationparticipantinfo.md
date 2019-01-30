---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641916"
---
# <a name="invitationparticipantinfo-resource-type"></a>invitationParticipantInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。

## <a name="properties"></a>属性

| 属性                           | 类型                          | 说明                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | String                        | 可取值为：`default`、`voicemail`。 |
| identity                           | [identitySet](identityset.md) | 与此邀请关联[identitySet](identityset.md) 。                   |
| languageId                         | String                        | 语言区域性字符串。                                                                                     |
| 区域                             | String                        | 参与者的区域。                                                           |
| replacesCallId                     | String                        | 可选。 呼叫的目标 idenity 目前的一部分。 一旦添加参与者，此呼叫将被丢弃。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
