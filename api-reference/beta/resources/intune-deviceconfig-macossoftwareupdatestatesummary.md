---
title: macOSSoftwareUpdateStateSummary 资源类型
description: MacOS 设备和用户的软件更新状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb7cebab56f9866753794259b70a0bdd8cc1e414
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279813"
---
# <a name="macossoftwareupdatestatesummary-resource-type"></a>macOSSoftwareUpdateStateSummary 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 设备和用户的软件更新状态摘要

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSSoftwareUpdateStateSummaries](../api/intune-deviceconfig-macossoftwareupdatestatesummary-list.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 集合|列出 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象的属性和关系。|
|[获取 macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|读取 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象的属性和关系。|
|[创建 macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|创建新的 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象。|
|[删除 macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|无|删除 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)。|
|[更新 macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|更新 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|displayName|字符串|人工可读名称的软件更新|
|productKey|String|软件更新的产品密钥。|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|软件更新类别。 可取值为：`critical`、`configurationDataFile`、`firmware`、`other`。|
|updateVersion|字符串|软件更新的版本|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|软件更新的状态。 可能的值为：、、、、、、、、、、、、、、 `success` `downloading` `downloaded` `installing` `idle` `available` `scheduled` `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` 。|
|lastUpdatedDateTime|DateTimeOffset|最后一次更新此设备和产品密钥的报告的日期。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "productKey": "String",
  "updateCategory": "String",
  "updateVersion": "String",
  "state": "String",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




