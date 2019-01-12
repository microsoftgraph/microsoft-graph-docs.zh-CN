---
title: embeddedSIMActivationCodePool 资源类型
description: 池代表嵌入 SIM 激活代码的一组。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c8265b0c8d0c0d83808741d90893bdec9b15825
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929751"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>embeddedSIMActivationCodePool 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

池代表嵌入 SIM 激活代码的一组。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)集合|列出属性和[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象之间的关系。|
|[获取 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|读取属性和[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象的关系。|
|[创建 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|创建新的[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象。|
|[删除 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|无|删除[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)。|
|[更新 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|更新[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象的属性。|
|[assign 操作](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|嵌入 SIM 激活代码池的的唯一标识符。 系统生成时创建分配值。|
|displayName|字符串|管理员定义的嵌入 SIM 激活代码池的名称。|
|createdDateTime|DateTimeOffset|嵌入的 SIM 激活代码池的创建时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|嵌入的 SIM 激活代码池上次修改时间。 更新服务端。|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)集合|属于此池激活代码。 此导航属性用于发布到 Intune 的激活代码，但不能用于读取 Intune 激活代码。|
|activationCodeCount|Int32|属于此池的激活代码的总计数。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)集合|导航属性设置为此池分配到的目标的列表。|
|deviceStates|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合|为此池的设备状态的列表的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```





