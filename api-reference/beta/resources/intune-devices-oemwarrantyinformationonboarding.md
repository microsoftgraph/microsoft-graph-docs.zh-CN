---
title: oemWarrantyInformationOnboarding 资源类型
description: 给定 OEM 的担保状态实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cfa2ba539f50fe7c550fe6b22cad7d88c7e265
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292361"
---
# <a name="oemwarrantyinformationonboarding-resource-type"></a>oemWarrantyInformationOnboarding 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定 OEM 的担保状态实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 oemWarrantyInformationOnboardings](../api/intune-devices-oemwarrantyinformationonboarding-list.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) 集合|列出 [oemWarrantyInformationOnboarding 对象的属性和](../resources/intune-devices-oemwarrantyinformationonboarding.md) 关系。|
|[获取 oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-get.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|读取 [oemWarrantyInformationOnboarding 对象的属性和](../resources/intune-devices-oemwarrantyinformationonboarding.md) 关系。|
|[创建 oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-create.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|创建新的 [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md) 对象。|
|[删除 oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-delete.md)|无|删除 [oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)。|
|[更新 oemWarrantyInformationOnboarding](../api/intune-devices-oemwarrantyinformationonboarding-update.md)|[oemWarrantyInformationOnboarding](../resources/intune-devices-oemwarrantyinformationonboarding.md)|更新 [oemWarrantyInformationOnboarding 对象](../resources/intune-devices-oemwarrantyinformationonboarding.md) 的属性。|
|[启用操作](../api/intune-devices-oemwarrantyinformationonboarding-enable.md)|无|尚未记录|
|[禁用操作](../api/intune-devices-oemwarrantyinformationonboarding-disable.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|OEM 担保状态的唯一标识符。 此属性是只读的。|
|oemName|String|OEM 名称。 此属性是只读的。|
|enabled|Boolean|指定是否对给定的 OEM 启用担保查询。 此属性是只读的。|
|可用|Boolean|指定是否提供担保 API。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oemWarrantyInformationOnboarding"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oemWarrantyInformationOnboarding",
  "id": "String (identifier)",
  "oemName": "String",
  "enabled": true,
  "available": true
}
```




