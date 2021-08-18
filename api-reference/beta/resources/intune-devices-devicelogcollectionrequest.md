---
title: deviceLogCollectionRequest 资源类型
description: WindowsLog Collection 请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f5de7a3b17e7c3f68e067d516dd008fc7464469c37a565bb23ba772d4013048
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133227"
---
# <a name="devicelogcollectionrequest-resource-type"></a>deviceLogCollectionRequest 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsLog Collection 请求实体。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一标识符|
|templateType|[deviceLogCollectionTemplateType](../resources/intune-devices-devicelogcollectiontemplatetype.md)|与集合请求一起发送的模板类型。 可能的值是 `predefined` ：。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```




