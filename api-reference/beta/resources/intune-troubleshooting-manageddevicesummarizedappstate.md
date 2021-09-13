---
title: managedDeviceSummarizedAppState 资源类型
description: 表示具有失败或挂起的应用的用户设备的事件。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 092dfef55500ec023c2cf0d79f63c5161c27c7c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057199"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a>managedDeviceSummarizedAppState 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示具有失败或挂起的应用的用户设备的事件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|summarizedAppState|[runState](../resources/intune-troubleshooting-runstate.md)|对象的 runState。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|deviceId|String|此对象表示的设备的设备 Id|

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




