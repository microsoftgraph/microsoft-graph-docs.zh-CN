---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4e8952012624a038f497fea3c6b81ad364448a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415339"
---
# <a name="ebookinstallsummary-resource-type"></a>eBookInstallSummary 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




