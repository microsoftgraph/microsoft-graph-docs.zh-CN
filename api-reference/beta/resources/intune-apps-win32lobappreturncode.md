---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34bda91a0374c57ef4f5ca6e51bc006c80592361
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975775"
---
# <a name="win32lobappreturncode-resource-type"></a>win32LobAppReturnCode 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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





