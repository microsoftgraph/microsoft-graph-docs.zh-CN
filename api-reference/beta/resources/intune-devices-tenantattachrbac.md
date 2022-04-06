---
title: tenantAttachRBAC 资源类型
description: 充当租户附加启用功能的容器的单一实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af582f15444821fba9e36cf23ef1f2c4075ad57c
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631179"
---
# <a name="tenantattachrbac-resource-type"></a>tenantAttachRBAC 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当租户附加启用功能的容器的单一实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 tenantAttachRBAC](../api/intune-devices-tenantattachrbac-get.md)|[tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md)|读取 [tenantAttachRBAC 对象的属性和](../resources/intune-devices-tenantattachrbac.md) 关系。|
|[更新 tenantAttachRBAC](../api/intune-devices-tenantattachrbac-update.md)|[tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md)|更新 [tenantAttachRBAC 对象](../resources/intune-devices-tenantattachrbac.md) 的属性。|
|[启用操作](../api/intune-devices-tenantattachrbac-enable.md)|无|尚未记录|
|[getState 函数](../api/intune-devices-tenantattachrbac-getstate.md)|[tenantAttachRBACState](../resources/intune-devices-tenantattachrbacstate.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantAttachRBAC"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantAttachRBAC",
  "id": "String (identifier)"
}
```




