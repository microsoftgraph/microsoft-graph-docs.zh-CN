---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01233111e74da95f84d0cbeb81e4675a5c6e049d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773194"
---
# <a name="detectedapp-resource-type"></a>detectedApp 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 detectedApps](../api/intune-devices-detectedapp-list.md)|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。|
|[获取 detectedApp](../api/intune-devices-detectedapp-get.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。|
|[创建 detectedApp](../api/intune-devices-detectedapp-create.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。|
|[删除 detectedApp](../api/intune-devices-detectedapp-delete.md)|无|删除 [detectedApp](../resources/intune-devices-detectedapp.md)。|
|[更新 detectedApp](../api/intune-devices-detectedapp-update.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|检测到的应用程序的唯一标识符。 创建此应用程序时，Intune 将自动生成它。 只读。|
|displayName|字符串|发现的应用程序的名称。 只读|
|version|String|发现的应用程序的版本。 只读|
|sizeInByte|Int64|发现的应用程序的大小，以字节为单位。 只读|
|deviceCount|Int32|已安装此应用程序的设备数量|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) 集合|已安装发现的应用程序的设备|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```





