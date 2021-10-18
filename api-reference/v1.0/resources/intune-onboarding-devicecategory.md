---
title: deviceCategory 资源类型
description: 设备类别提供了整理设备的方法。 公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 623bb0c9eba0c46bacbcb06aba3d319c1cb98768
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450191"
---
# <a name="devicecategory-resource-type"></a>deviceCategory 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备类别提供了整理设备的方法。 公司管理员可以使用设备类别定义对其公司有意义的属于他们自己的类别。 然后可将这些类别应用于 Intune Azure 控制台中的设备，或在用户注册设备时供他们选择。 可以根据设备类别筛选报告并创建动态 Azure Active Directory 设备组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List deviceCategories](../api/intune-onboarding-devicecategory-list.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md) 集合|列出 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象的属性和关系。|
|[Get deviceCategory](../api/intune-onboarding-devicecategory-get.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|读取 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象的属性和关系。|
|[Create deviceCategory](../api/intune-onboarding-devicecategory-create.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|创建新的 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象。|
|[Delete deviceCategory](../api/intune-onboarding-devicecategory-delete.md)|无|删除 [deviceCategory](../resources/intune-onboarding-devicecategory.md)。|
|[Update deviceCategory](../api/intune-onboarding-devicecategory-update.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|更新 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备类别的唯一标识符。 只读。|
|displayName|String|设备类别的显示名称。|
|说明|String|设备类别的说明（可选）。|

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



