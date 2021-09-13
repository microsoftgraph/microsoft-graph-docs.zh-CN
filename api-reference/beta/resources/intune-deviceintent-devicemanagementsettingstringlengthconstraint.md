---
title: deviceManagementSettingStringLengthConstraint 资源类型
description: 强制给定字符串长度范围的约束
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2cda4436f30fb1fc4a0f33b7f180691463fc8c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091375"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a>deviceManagementSettingStringLengthConstraint 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

强制给定字符串长度范围的约束


继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|minimumLength|Int32|允许的最小字符串长度|
|maximumLength|Int32|允许的最大字符串长度|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



