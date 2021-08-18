---
title: deviceCategory 资源类型
description: 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1e30c9154208fc4f7bae9d5dbcb7a4104c4651343f87df0f620d20901f470f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219743"
---
# <a name="devicecategory-resource-type"></a>deviceCategory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备类别提供了一种组织设备的方法。 使用设备类别，公司管理员可以定义对公司有意义的独特类别。 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List deviceCategories](../api/intune-shared-devicecategory-list.md)|[deviceCategory](../resources/intune-shared-devicecategory.md) 集合|列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。|
|[Get deviceCategory](../api/intune-shared-devicecategory-get.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|读取 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。|
|[Create deviceCategory](../api/intune-shared-devicecategory-create.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。|
|[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md)|无|删除 [deviceCategory](../resources/intune-shared-devicecategory.md)。|
|[Update deviceCategory](../api/intune-shared-devicecategory-update.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|更新 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备类别的唯一标识符。 只读。|
|**载入**|
|displayName|字符串|设备类别的显示名称。|
|description|String|设备类别的说明（可选）。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```




