---
title: managedDeviceSummarizedAppState 资源类型
description: 表示具有失败或挂起的应用程序的用户设备的事件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4727477497657a917906f9b778fa76647fc394d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271602"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a>managedDeviceSummarizedAppState 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示具有失败或挂起的应用程序的用户设备的事件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|summarizedAppState|[runState](../resources/intune-shared-runstate.md)|对象的 runState。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|deviceId|String|此对象表示的设备的 DeviceId|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```




