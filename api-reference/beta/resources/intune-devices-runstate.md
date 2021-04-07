---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612183"
---
# <a name="runstate-enum-type"></a>runState 枚举类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|unknown|0|结果未知。|
|success|1|脚本成功运行。|
|失败|2|脚本无法运行。|
|scriptError|3|发现脚本命中错误。|
|pending|4 |脚本正在等待执行。|
|notApplicable|5 |脚本不适用于此设备。|




