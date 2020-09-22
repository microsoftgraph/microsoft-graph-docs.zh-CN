---
title: roleManagement 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40a74c46f02aef42c8785e666705278980c544c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021495"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 roleManagement](../api/intune-rbac-rolemanagement-get.md)|[roleManagement](../resources/intune-rbac-rolemanagement.md)|读取 [roleManagement](../resources/intune-rbac-rolemanagement.md) 对象的属性和关系。|
|[更新 roleManagement](../api/intune-rbac-rolemanagement-update.md)|[roleManagement](../resources/intune-rbac-rolemanagement.md)|更新 [roleManagement](../resources/intune-rbac-rolemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceManagement|[rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)|RbacApplication 的设备管理|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "String (identifier)"
}
```






