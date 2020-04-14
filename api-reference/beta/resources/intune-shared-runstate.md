---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 37905590f5ca61db53f98ff047ef699549f269ae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473506"
---
# <a name="runstate-enum-type"></a>runState 枚举类型

命名空间：microsoft.graph

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



