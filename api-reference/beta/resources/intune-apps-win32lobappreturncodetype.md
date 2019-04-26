---
title: win32LobAppReturnCodeType 枚举类型
description: 指示返回代码的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 441c0270bc6488a09fec02f1e1681e009b889918
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556891"
---
# <a name="win32lobappreturncodetype-enum-type"></a>win32LobAppReturnCodeType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示返回代码的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|未能|0|未能.|
|success|1|成功.|
|softReboot|2 |软重启是必需的。|
|hardReboot|3 |需要进行硬重新启动。|
|稍后|4 |再重试。|





