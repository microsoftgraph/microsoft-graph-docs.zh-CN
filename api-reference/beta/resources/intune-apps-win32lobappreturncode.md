---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4402464bd4618f1e33b9b766be529cbe592165c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174585"
---
# <a name="win32lobappreturncode-resource-type"></a>win32LobAppReturnCode 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Win32 应用的返回代码属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|returnCode|Int32|返回代码。|
|type|[win32LobAppReturnCodeType](../resources/intune-apps-win32lobappreturncodetype.md)|返回代码的类型。 可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```




