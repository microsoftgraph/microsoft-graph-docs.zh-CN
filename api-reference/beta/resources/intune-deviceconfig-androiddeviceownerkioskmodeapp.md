---
title: androidDeviceOwnerKioskModeApp 资源类型
description: Android 设备所有者托管主屏幕上的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: add6b78cab85abc315efe41d5bd885298f0015aed1630036c061417feeeae19b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245126"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a>androidDeviceOwnerKioskModeApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者托管主屏幕上的应用程序


继承自 [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|package|字符串|应用程序的程序包名称|
|className|String|应用程序的类名称|

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




