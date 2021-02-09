---
title: androidDeviceOwnerKioskModeManagedFolder 资源类型
description: 一个文件夹，其中包含托管主屏幕上的应用页面和 Web 链接
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4e6b373729ffebb3fc7a08ee29e98f3471c8c27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162264"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a>androidDeviceOwnerKioskModeManagedFolder 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个文件夹，其中包含托管主屏幕上的应用页面和 Web 链接

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|folderName|String|文件夹的显示名称|
|folderIdentifier|String|文件夹的唯一标识符|
|items|[androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md) 集合|要添加到托管文件夹的项目。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
  "folderName": "String",
  "folderIdentifier": "String",
  "items": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
      "label": "String",
      "link": "String"
    }
  ]
}
```




