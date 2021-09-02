---
title: embeddedSIMActivationCodePool 资源类型
description: 池表示一组嵌入式 SIM 卡激活代码。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9579f4af46ca2b35fde91888ced9973590634095
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801071"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>embeddedSIMActivationCodePool 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

池表示一组嵌入式 SIM 卡激活代码。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 集合|列出 [embeddedSIMActivationCodePool 对象的属性和](../resources/intune-esim-embeddedsimactivationcodepool.md) 关系。|
|[获取 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|读取 [embeddedSIMActivationCodePool 对象的属性和](../resources/intune-esim-embeddedsimactivationcodepool.md) 关系。|
|[创建 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|创建新的 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象。|
|[删除 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|无|删除嵌入式 [SIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)。|
|[更新 embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|更新嵌入式 [SIMActivationCodePool 对象](../resources/intune-esim-embeddedsimactivationcodepool.md) 的属性。|
|[分配操作](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|嵌入式 SIM 卡激活代码池的唯一标识符。 创建时分配的系统生成值。|
|displayName|String|管理员定义的嵌入式 SIM 卡激活代码池的名称。|
|createdDateTime|DateTimeOffset|嵌入式 SIM 卡激活代码池的创建时间。 生成的服务器端。|
|modifiedDateTime|DateTimeOffset|上次修改嵌入式 SIM 卡激活代码池的时间。 更新的服务器端。|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) 集合|属于此池的激活代码。 此导航属性用于将激活代码张贴到 Intune，但不能用于从 Intune 读取激活代码。|
|activationCodeCount|Int32|属于此池的激活代码总数。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 集合|分配给此池的目标列表的导航属性。|
|deviceStates|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) 集合|此池的设备状态列表的导航属性。|

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



