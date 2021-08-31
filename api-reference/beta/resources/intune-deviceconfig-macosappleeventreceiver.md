---
title: macOSAppleEventReceiver 资源类型
description: 表示可以接收 Apple 事件通知的过程。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14f68bfa31c41b96e2a2dd160fa732d2c38e9b2f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58810645"
---
# <a name="macosappleeventreceiver-resource-type"></a>macOSAppleEventReceiver 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示可以接收 Apple 事件通知的过程。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|codeRequirement|String|接收 Apple 事件的应用或二进制文件的代码要求。|
|标识符|String|接收 Apple 事件的进程或可执行文件的应用或文件路径的捆绑 ID。|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|将应用或路径的捆绑 ID 用于接收 Apple 事件的进程或可执行文件。 可取值为：`bundleID`、`path`。|
|allowed|Boolean|允许或阻止此应用程序接收 Apple 事件。|

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



