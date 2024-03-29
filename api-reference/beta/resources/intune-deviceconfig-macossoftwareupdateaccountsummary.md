---
title: macOSSoftwareUpdateAccountSummary 资源类型
description: 设备和用户的 MacOS 软件更新帐户摘要报告
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 467ee509de4b8cdd147328fd20686060d1a8b7d8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009090"
---
# <a name="macossoftwareupdateaccountsummary-resource-type"></a>macOSSoftwareUpdateAccountSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备和用户的 MacOS 软件更新帐户摘要报告

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSSoftwareUpdateAccountSummaries](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-list.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 集合|列出 [macOSSoftwareUpdateAccountSummary 对象的属性和](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 关系。|
|[获取 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-get.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|读取 [macOSSoftwareUpdateAccountSummary 对象的属性和](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 关系。|
|[创建 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-create.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|创建新的 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 对象。|
|[删除 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-delete.md)|None|删除 [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)。|
|[更新 macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-update.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|更新 [macOSSoftwareUpdateAccountSummary 对象](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|报告的名称|
|deviceId|String|设备 ID。|
|userId|String|用户 ID。|
|deviceName|String|设备名称。|
|userPrincipalName|String|用户主体名称|
|osVersion|String|操作系统版本。|
|successfulUpdateCount|Int32|设备上成功更新的数量。|
|failedUpdateCount|Int32|设备上失败的更新数。|
|totalUpdateCount|Int32|设备上的总更新数。|
|lastUpdatedDateTime|DateTimeOffset|上次更新此设备的报告的日期时间。|

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



