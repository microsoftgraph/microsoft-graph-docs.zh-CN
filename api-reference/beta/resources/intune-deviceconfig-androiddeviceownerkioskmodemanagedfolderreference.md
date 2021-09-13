---
title: androidDeviceOwnerKioskModeManagedFolderReference 资源类型
description: 对托管主屏幕上包含应用和 Web 链接的文件夹的引用
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97276755676fbde8e41d4c5bac3fb1e381b7376d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030450"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a>androidDeviceOwnerKioskModeManagedFolderReference 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对托管主屏幕上包含应用和 Web 链接的文件夹的引用


继承自 [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|folderName|String|文件夹的名称|
|folderIdentifier|String|文件夹的唯一标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference",
  "folderName": "String",
  "folderIdentifier": "String"
}
```



