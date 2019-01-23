---
title: embeddedSIMActivationCodePool 资源类型
description: 池代表嵌入 SIM 激活代码的一组。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9dfcca046abf206fc29bbc6033bbd88980f9bf43
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410614"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>embeddedSIMActivationCodePool 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|id|String|嵌入 SIM 激活代码池的的唯一标识符。 系统生成时创建分配值。|
|displayName|String|管理员定义的嵌入 SIM 激活代码池的名称。|
|createdDateTime|DateTimeOffset|嵌入的 SIM 激活代码池的创建时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|嵌入的 SIM 激活代码池上次修改时间。 更新服务端。|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)集合|属于此池激活代码。 此导航属性用于发布到 Intune 的激活代码，但不能用于读取 Intune 激活代码。|
|activationCodeCount|Int32|属于此池的激活代码的总计数。|

## <a name="relationships"></a>关系
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




