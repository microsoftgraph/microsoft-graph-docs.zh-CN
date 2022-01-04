---
title: configurationManagerAction 资源类型
description: 操作 triggerConfigurationManagerAction 的参数
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07cf57cf159b9a30dc653a0cbe26451b97b903fe
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711912"
---
# <a name="configurationmanageraction-resource-type"></a>configurationManagerAction 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作 triggerConfigurationManagerAction 的参数

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|[configurationManagerActionType](../resources/intune-devices-configurationmanageractiontype.md)|在 Configuration Manager 客户端上触发的操作类型。 可取值为：`refreshMachinePolicy`、`refreshUserPolicy`、`wakeUpClient`、`appEvaluation`、`quickScan`、`fullScan`、`windowsDefenderUpdateSignatures`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerAction",
  "action": "String"
}
```




