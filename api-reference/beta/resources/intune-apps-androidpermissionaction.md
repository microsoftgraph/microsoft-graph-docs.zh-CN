---
title: androidPermissionAction 资源类型
description: 在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0e1b793a447d29d1ed554e1b6466895ccc9e57f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459140"
---
# <a name="androidpermissionaction-resource-type"></a>androidPermissionAction 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|拒绝|String|Android 权限字符串，在官方 Android 文档中定义。  示例 "android. READ_CONTACTS"。|
|action|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Android 权限操作的类型。 可取值为：`prompt`、`autoGrant`、`autoDeny`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```



