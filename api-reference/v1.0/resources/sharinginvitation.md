---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 9237c401fd83a7b30303f147402262c022b820a7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265853"
---
# <a name="sharinginvitation-resource-type"></a>SharingInvitation 资源类型

**SharingInvitation** 资源将与邀请相关的数据项分组到一个单一结构。

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

| 属性名称  | 类型            | 说明
|:---------------|:----------------|:------------------------------------------
| email          | 字符串          | 为共享邀请的收件人提供的电子邮件地址。只读。
| invitedBy      | [identitySet][] | 提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。
| signInRequired | 布尔         | 如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

[DriveItem]: driveItem.md
[IdentitySet]: identitySet.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
