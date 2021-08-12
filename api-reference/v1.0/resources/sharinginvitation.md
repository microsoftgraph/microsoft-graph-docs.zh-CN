---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: SharingInvitation 资源将邀请相关的数据项分组到一个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eaf917ccdd64a50dab9cdf6f2ed477716c18a0185be03812793d115247e17e93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134936"
---
# <a name="sharinginvitation-resource-type"></a>SharingInvitation 资源类型

命名空间：microsoft.graph

**SharingInvitation** 资源将邀请相关的数据项分组到一个结构中。

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

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/SharingInvitation"
} -->

