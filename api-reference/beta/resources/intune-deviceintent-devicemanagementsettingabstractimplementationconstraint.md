---
title: deviceManagementSettingAbstractImplementationConstraint 资源类型
description: 强制使用 AbstractComplex 类型的约束具有或设置为特定值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0b3956b78ef63f1b6d7d15f4d5b51a0225b92334643935ef1050aa4e70be456
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252905"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a>deviceManagementSettingAbstractImplementationConstraint 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

强制使用 AbstractComplex 类型的约束具有或设置为特定值


继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAbstractImplementationDefinitionIds|String collection|值列表，表示未针对设置进行配置|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAbstractImplementationConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAbstractImplementationConstraint",
  "allowedAbstractImplementationDefinitionIds": [
    "String"
  ]
}
```




