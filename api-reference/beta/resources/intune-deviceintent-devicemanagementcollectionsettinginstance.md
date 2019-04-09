---
title: deviceManagementCollectionSettingInstance 资源类型
description: 一个代表值集合的设置实例
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31ce38adb753354c319a27e55cad8aa8a1e6024e
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524545"
---
# <a name="devicemanagementcollectionsettinginstance-resource-type"></a>deviceManagementCollectionSettingInstance 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个代表值集合的设置实例


继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementCollectionSettingInstances](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-list.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)集合|列出[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的属性和关系。|
|[获取 deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-get.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|读取[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的属性和关系。|
|[创建 deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-create.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|创建新的[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。|
|[删除 deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-delete.md)|无|删除[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)。|
|[更新 deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-update.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|更新[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID|
|definitionId|String|继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID|
|valueJson|String|继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|value|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合|值的集合|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```







