---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 067e7894cc5c5daa4cd73c5bb5ba88f66b283366
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732363"
---
# <a name="devicecategory-resource-type"></a>deviceCategory 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备类别提供了整理设备的方法。 公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 deviceCategories](../api/intune-shared-devicecategory-list.md) 集合|列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。|
|[Get deviceCategory](../api/intune-shared-devicecategory-get.md)|读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。|
|[Create deviceCategory](../api/intune-shared-devicecategory-create.md)|创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。|
|[删除 deviceCategory](../api/intune-shared-devicecategory-delete.md)。|
|[Update deviceCategory](../api/intune-shared-devicecategory-update.md)|更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备类别的唯一标识符。 只读。|
|**载入**|
|displayName|String|设备类别的显示名称。|
|说明|String|设备类别的说明（可选）。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```









