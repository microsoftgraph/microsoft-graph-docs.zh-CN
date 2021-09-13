---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf03fc1712e2edfca1a5d51ed025ba8a1c1fba99
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095701"
---
# <a name="ebookinstallsummary-resource-type"></a>eBookInstallSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含某个设备的书籍安装摘要的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 eBookInstallSummary](../api/intune-books-ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。|
|[更新 eBookInstallSummary](../api/intune-books-ebookinstallsummary-update.md)|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|installedDeviceCount|Int32|已成功安装此书籍的设备数量。|
|failedDeviceCount|Int32|未能成功安装此书籍的设备数量。|
|notInstalledDeviceCount|Int32|未安装此书籍的设备数量。|
|installedUserCount|Int32|其设备全部成功安装了此书籍的用户数量。|
|failedUserCount|Int32|有 1 个或多个设备未能安装此书籍的用户数量。|
|notInstalledUserCount|Int32|未安装此书籍的用户数量。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



