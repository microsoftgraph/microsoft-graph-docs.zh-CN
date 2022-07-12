---
author: JeremyKelley
description: SharingInvitation 资源将邀请相关的数据项分组到单个结构中。
ms.date: 09/10/2017
title: SharingInvitation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: d13950d9662504e3058b40fafdd9c192e825baea
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732700"
---
# <a name="sharinginvitation-resource-type"></a>SharingInvitation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**SharingInvitation** 资源将邀请相关的数据项分组到单个结构中。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a>属性

| 属性       | 类型                          | 说明                                                                                                                   |
| :------------- | :---------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| email          | String                        | 为共享邀请的收件人提供的电子邮件地址。只读。                                            |
| invitedBy      | [identitySet](identityset.md) | 提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。 |
| signInRequired | Boolean                       | 如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。                     |

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
