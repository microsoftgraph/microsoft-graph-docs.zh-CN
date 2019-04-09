---
title: securityBaselineState 资源类型
description: 设备的安全基准状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c81a3d351c7c1e854c26e05e32f8426ffdc0631
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524559"
---
# <a name="securitybaselinestate-resource-type"></a>securityBaselineState 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备的安全基准状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityBaselineStates](../api/intune-deviceintent-securitybaselinestate-list.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)集合|列出[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性和关系。|
|[获取 securityBaselineState](../api/intune-deviceintent-securitybaselinestate-get.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|读取[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性和关系。|
|[创建 securityBaselineState](../api/intune-deviceintent-securitybaselinestate-create.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|创建新的[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。|
|[删除 securityBaselineState](../api/intune-deviceintent-securitybaselinestate-delete.md)|无|删除[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)。|
|[更新 securityBaselineState](../api/intune-deviceintent-securitybaselinestate-update.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|更新[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|securityBaselineTemplateId|String|安全基准模板 id|
|displayName|String|安全基准的显示名称|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settingStates|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)集合|设备的不同设置的安全基准状态|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```



