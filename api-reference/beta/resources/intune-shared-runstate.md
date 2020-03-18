---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f4c1605734afef3caefc4b51e2c8a826d2f2cd4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767818"
---
# <a name="runstate-enum-type"></a>runState 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知结果。|
|success|1|脚本成功运行。|
|失败|双面|脚本运行失败。|
|scriptError|第三章|发现脚本命中错误。|
|决|4 |脚本正在挂起中执行。|
|notApplicable|5 |脚本不适用于此设备。|



