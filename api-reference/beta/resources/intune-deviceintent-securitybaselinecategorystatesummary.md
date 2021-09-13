---
title: securityBaselineCategoryStateSummary 资源类型
description: 每个类别合规性状态的安全基线帐户的安全基线摘要。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab4ed7a5d2b8c32114fc6e222f5a605a2bc7e059
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051277"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a>securityBaselineCategoryStateSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每个类别合规性状态的安全基线帐户的安全基线摘要。


继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityBaselineCategoryStateSummaries](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 集合|列出 [securityBaselineCategoryStateSummary 对象的属性和](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 关系。|
|[获取 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|读取 [securityBaselineCategoryStateSummary 对象的属性和](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 关系。|
|[创建 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|创建新的 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。|
|[删除 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|无|删除 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)。|
|[更新 securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|更新 [securityBaselineCategoryStateSummary 对象](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|secureCount|Int32|安全设备的数量 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notSecureCount|Int32|非安全设备的数量 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|unknownCount|Int32|未知设备数 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|errorCount|Int32|错误设备数 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|conflictCount|Int32|冲突设备数 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notApplicableCount|Int32|不适用的设备数 继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
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



