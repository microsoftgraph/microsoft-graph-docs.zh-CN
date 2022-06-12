---
author: JeremyKelley
ms.date: 09/10/2017
title: sharingInvitation 资源类型
ms.localizationpriority: medium
description: sharingInvitation 资源将邀请相关的数据项分组到单个结构中。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 7c76fe60f21831db94b44df5f6e0ccabdeff98d8
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034934"
---
# <a name="sharinginvitation-resource-type"></a>sharingInvitation 资源类型

命名空间：microsoft.graph

将邀请相关的数据项分组到单个结构中。

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

| 属性名  | 类型            | 说明
|:---------------|:----------------|:------------------------------------------
| email          | String          | 为共享邀请的收件人提供的电子邮件地址。只读。
| invitedBy      | [identitySet][] | 提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。
| signInRequired | Boolean         | 如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/SharingInvitation"
} -->

