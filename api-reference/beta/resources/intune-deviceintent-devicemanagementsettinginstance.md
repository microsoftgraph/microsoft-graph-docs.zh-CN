---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28f380bc2aef749079676d4f97fd4bd6f3d7c671
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364647"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>deviceManagementSettingInstance 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设置实例的基本类型

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementSettingInstances](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合|列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。|
|[获取 deviceManagementSettingInstance](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。|

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



