---
title: officeClientConfigurationAssignment 资源类型
description: Office客户端配置分配。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b14d12e3001d66724c1ebe94ba73e9797f7d9ac0
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819042"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>officeClientConfigurationAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Office客户端配置分配。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 officeClientConfigurationAssignments](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 集合|列出 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象的属性和关系。|
|[获取 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|读取 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象的属性和关系。|
|[创建 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|创建新的 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象。|
|[删除 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|无|删除 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)。|
|[更新 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|更新 [officeClientConfigurationAssignment 对象](../resources/intune-cirrus-officeclientconfigurationassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|OfficeConfigurationAssignment 的 ID。|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|由管理员定义的目标分配。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



