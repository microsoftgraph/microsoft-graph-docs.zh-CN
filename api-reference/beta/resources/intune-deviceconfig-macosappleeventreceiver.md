---
title: macOSAppleEventReceiver 资源类型
description: 表示可以接收 Apple 事件通知的过程。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03dd639dbd23d10dbaf859a156badd7fec63a0fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268963"
---
# <a name="macosappleeventreceiver-resource-type"></a>macOSAppleEventReceiver 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示可以接收 Apple 事件通知的过程。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|codeRequirement|字符串|接收 Apple 事件的应用程序或二进制文件的代码要求。|
|标识符|字符串|接收 Apple 事件的进程或可执行文件的应用程序或文件路径的捆绑包 ID。|
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




