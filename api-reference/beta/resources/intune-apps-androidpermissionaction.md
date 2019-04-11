---
title: androidPermissionAction 资源类型
description: 在请求该权限时, android 应用程序权限和适用于 android 的操作之间的映射应采取的操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fec33b2600e88e6a4dfae644c335d9652c20abe0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792963"
---
# <a name="androidpermissionaction-resource-type"></a>androidPermissionAction 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在请求该权限时, android 应用程序权限和适用于 android 的操作之间的映射应采取的操作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|拒绝|String|android 权限字符串, 在官方 android 文档中定义。  示例 "READ_CONTACTS"。|
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





