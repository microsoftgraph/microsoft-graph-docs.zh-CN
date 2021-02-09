---
title: androidDeviceOwnerKioskModeApp 资源类型
description: Android 设备所有者托管主屏幕上的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da6adb416c8fd20406c295e56a5d15177e625c30
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160556"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a>androidDeviceOwnerKioskModeApp 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者托管主屏幕上的应用程序


继承自 [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|package|String|应用程序的程序包名称|
|className|String|应用程序的类名|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeApp",
  "package": "String",
  "className": "String"
}
```




