---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基类型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f56f518a8d45f93c25e8c450ce4152d7d7a38964
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134897"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>deviceManagementSettingInstance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设置实例的基类型

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementSettingInstances](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 集合|列出 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 对象的属性和关系。|
|[获取 deviceManagementSettingInstance](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|读取 [deviceManagementSettingInstance 对象的属性和](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置实例 ID|
|definitionId|String|此实例的设置定义的 ID|
|valueJson|String|值的 JSON 表示形式|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



