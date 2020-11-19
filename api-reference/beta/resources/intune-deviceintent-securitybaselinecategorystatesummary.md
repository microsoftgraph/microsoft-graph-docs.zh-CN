---
title: securityBaselineCategoryStateSummary 资源类型
description: 帐户安全基准的每个类别合规性状态摘要的安全基准。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: acf1eecb183bd9d0a69caa087f017cc878bc252a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209386"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a>securityBaselineCategoryStateSummary 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户安全基准的每个类别合规性状态摘要的安全基准。


继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityBaselineCategoryStateSummaries](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 集合|列出 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象的属性和关系。|
|[获取 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|读取 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象的属性和关系。|
|[创建 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|创建新的 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。|
|[删除 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|无|删除 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)。|
|[更新 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|更新 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|secureCount|Int32|继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的安全设备的数量|
|notSecureCount|Int32|从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不安全设备的数量|
|unknownCount|Int32|从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的未知设备的数量|
|errorCount|Int32|继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的错误设备的数量|
|conflictCount|Int32|继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的冲突设备的数量|
|notApplicableCount|Int32|从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不适用设备的数量|
|displayName|String|类别名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```




