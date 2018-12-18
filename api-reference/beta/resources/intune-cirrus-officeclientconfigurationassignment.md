---
title: officeClientConfigurationAssignment 资源类型
description: Office 客户端配置工作分配。
author: tfitzmac
ms.openlocfilehash: c2b8dc231fb390cbb2bd5dbb93b5226540b84f5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315991"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>officeClientConfigurationAssignment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Office 客户端配置工作分配。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 officeClientConfigurationAssignments](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合|列出属性和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象之间的关系。|
|[获取 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|读取属性和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的关系。|
|[创建 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|创建新的[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。|
|[删除 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|无|删除[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)。|
|[更新 officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|更新[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|OfficeConfigurationAssignment 的 id。|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|目标工作分配定义的管理员。|

## <a name="relationships"></a>Relationships
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



