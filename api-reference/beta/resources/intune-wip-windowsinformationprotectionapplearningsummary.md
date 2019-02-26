---
title: windowsInformationProtectionAppLearningSummary 资源类型
description: Windows 信息保护应用学习摘要实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c42fbe9da221e9c41a29291d6a279b1144cd355
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169487"
---
# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>windowsInformationProtectionAppLearningSummary 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 信息保护应用学习摘要实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsInformationProtectionAppLearningSummaries](../api/intune-wip-windowsinformationprotectionapplearningsummary-list.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 集合|列出 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性和关系。|
|[获取 windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|读取 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性和关系。|
|[创建 windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。|
|[删除 windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-delete.md)|无|删除 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)。|
|[更新 windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|更新 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|WindowsInformationProtectionAppLearningSummary 的唯一标识符。|
|applicationName|String|应用程序名称|
|applicationType|[applicationType](../resources/intune-wip-applicationtype.md)|应用程序类型。 可取值为：`universal`、`desktop`。|
|deviceCount|Int32|设备计数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```




