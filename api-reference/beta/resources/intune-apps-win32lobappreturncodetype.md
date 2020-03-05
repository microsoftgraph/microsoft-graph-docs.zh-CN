---
title: win32LobAppReturnCodeType 枚举类型
description: 指示返回代码的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d97896382ef5b596cdded326f3579f746d9b09b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490257"
---
# <a name="win32lobappreturncodetype-enum-type"></a>win32LobAppReturnCodeType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示返回代码的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|未能|0|未能.|
|success|1 |成功.|
|softReboot|2 |软重启是必需的。|
|hardReboot|3 |需要进行硬重新启动。|
|稍后|4 |再重试。|



