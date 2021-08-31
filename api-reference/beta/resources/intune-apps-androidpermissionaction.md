---
title: androidPermissionAction 资源类型
description: Android 应用权限与 Android 在请求该权限时应执行的操作之间的映射。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d99ec168ae3cdb46dbe7727e9b60fb63624202fe
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819729"
---
# <a name="androidpermissionaction-resource-type"></a>androidPermissionAction 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 应用权限与 Android 在请求该权限时应执行的操作之间的映射。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|permission|String|Android 权限字符串，在官方 Android 文档中定义。  示例"android.permission.READ_CONTACTS"。|
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



