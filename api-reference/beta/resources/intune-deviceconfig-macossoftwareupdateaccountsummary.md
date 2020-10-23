---
title: macOSSoftwareUpdateAccountSummary 资源类型
description: MacOS 设备和用户的软件更新帐户摘要报告
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46a7cf012954189a3c14bdcdb6364ed9557d7f84
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727468"
---
# <a name="macossoftwareupdateaccountsummary-resource-type"></a>macOSSoftwareUpdateAccountSummary 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 设备和用户的软件更新帐户摘要报告

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSSoftwareUpdateAccountSummaries](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-list.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 集合|列出 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象的属性和关系。|
|[获取 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-get.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|读取 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象的属性和关系。|
|[创建 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-create.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|创建新的 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象。|
|[删除 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-delete.md)|无|删除 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)。|
|[更新 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-update.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|更新 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|报告的名称|
|deviceId|String|设备 ID。|
|userId|String|用户 ID。|
|deviceName|String|设备名称。|
|userPrincipalName|String|用户主体名称|
|osVersion|String|OS 版本。|
|successfulUpdateCount|Int32|设备上的成功更新数。|
|failedUpdateCount|Int32|设备上的失败更新数。|
|totalUpdateCount|Int32|设备上的总更新数。|
|lastUpdatedDateTime|DateTimeOffset|最后一次更新此设备的报告的日期。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categorySummaries|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) 集合|按类别分类的更新摘要。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateAccountSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceName": "String",
  "userPrincipalName": "String",
  "osVersion": "String",
  "successfulUpdateCount": 1024,
  "failedUpdateCount": 1024,
  "totalUpdateCount": 1024,
  "lastUpdatedDateTime": "String (timestamp)"
}
```





