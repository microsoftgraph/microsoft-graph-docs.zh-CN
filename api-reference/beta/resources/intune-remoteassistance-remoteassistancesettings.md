---
title: remoteAssistanceSettings 资源类型
description: 帐户的远程协助设置
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0179aaeb870c49c89bbb7795a1cc7962011dac68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039453"
---
# <a name="remoteassistancesettings-resource-type"></a>remoteAssistanceSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户的远程协助设置

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 remoteAssistanceSettings](../api/intune-remoteassistance-remoteassistancesettings-get.md)|[remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md)|读取 [remoteAssistanceSettings 对象的属性和](../resources/intune-remoteassistance-remoteassistancesettings.md) 关系。|
|[更新 remoteAssistanceSettings](../api/intune-remoteassistance-remoteassistancesettings-update.md)|[remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md)|更新 [remoteAssistanceSettings 对象](../resources/intune-remoteassistance-remoteassistancesettings.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|远程协助设置标识符|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|帐户的远程协助的当前状态。 可能的值包括：notConfigured、disabled、enabled。 管理员可以配置此设置。管理员尚未配置的远程协助设置具有 notConfigured 状态。 默认情况下返回。 可取值为：`notConfigured`、`disabled`、`enabled`。|
|allowSessionsToUnenrolledDevices|Boolean| 指示是否允许帐户使用到注销设备的会话。 管理员可以配置此设置。默认值为 false。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistanceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "id": "String (identifier)",
  "remoteAssistanceState": "String",
  "allowSessionsToUnenrolledDevices": true
}
```



