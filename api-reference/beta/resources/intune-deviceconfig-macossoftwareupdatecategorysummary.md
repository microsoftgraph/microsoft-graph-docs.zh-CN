---
title: macOSSoftwareUpdateCategorySummary 资源类型
description: 设备和用户的 MacOS 软件更新类别摘要报告
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f8d084eccf6e253c258f7ddd14c1c09feaa1ad2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095561"
---
# <a name="macossoftwareupdatecategorysummary-resource-type"></a>macOSSoftwareUpdateCategorySummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备和用户的 MacOS 软件更新类别摘要报告

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSSoftwareUpdateCategorySummaries](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-list.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 集合|列出 [macOSSoftwareUpdateCategorySummary 对象的属性和](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 关系。|
|[获取 macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-get.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|读取 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象的属性和关系。|
|[创建 macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-create.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|创建新的 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 对象。|
|[删除 macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-delete.md)|无|删除 [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)。|
|[更新 macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-update.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|更新 [macOSSoftwareUpdateCategorySummary 对象](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|报告的名称|
|deviceId|String|设备 ID。|
|userId|String|用户 ID。|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|软件更新类型。 可取值为：`critical`、`configurationDataFile`、`firmware`、`other`。|
|successfulUpdateCount|Int32|设备上成功更新的数量|
|failedUpdateCount|Int32|设备上失败的更新数|
|totalUpdateCount|Int32|设备上的总更新数|
|lastUpdatedDateTime|DateTimeOffset|上次更新此设备的报告的日期时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|updateStateSummaries|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 集合|更新状态摘要。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateCategorySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "String (identifier)",
  "displayName": "String",
  "deviceId": "String",
  "userId": "String",
  "updateCategory": "String",
  "successfulUpdateCount": 1024,
  "failedUpdateCount": 1024,
  "totalUpdateCount": 1024,
  "lastUpdatedDateTime": "String (timestamp)"
}
```



