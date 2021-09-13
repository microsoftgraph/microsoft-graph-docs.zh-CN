---
title: deviceManagementConfigurationDependentOn 资源类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f216b43ae577d670763a3fe3c2b26f3a14d84072
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128947"
---
# <a name="devicemanagementconfigurationdependenton-resource-type"></a>deviceManagementConfigurationDependentOn 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|dependentOn|String|取决于父设置/父设置选项的标识符|
|parentSettingId|String|依赖的父设置/父设置 ID 的标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationDependentOn",
  "dependentOn": "String",
  "parentSettingId": "String"
}
```



