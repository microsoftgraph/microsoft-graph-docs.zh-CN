---
title: macOSAppleEventReceiver 资源类型
description: 表示可以接收 Apple 事件通知的过程。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db781ad536e8fe918257f74d87fa104f4b2a23f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055447"
---
# <a name="macosappleeventreceiver-resource-type"></a>macOSAppleEventReceiver 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示可以接收 Apple 事件通知的过程。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|codeRequirement|String|接收 Apple 事件的应用程序或二进制文件的代码要求。|
|标识符|String|接收 Apple 事件的进程或可执行文件的应用程序或文件路径的捆绑包 ID。|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|对接收 Apple 事件的进程或可执行文件使用应用程序或路径的捆绑包 ID。 可取值为：`bundleID`、`path`。|
|支持|Boolean|允许或阻止此应用接收 Apple 事件。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```






