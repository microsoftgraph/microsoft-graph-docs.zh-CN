---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d3a5d1ce5c05d0a8c20a79aea2fd3562ab2170c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915940"
---
# <a name="ebookinstallsummary-resource-type"></a>eBookInstallSummary 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





