---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f25057c0fcd19b3a9ad121471876f7b6f1e5d15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020173"
---
# <a name="runstate-enum-type"></a>runState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|结果未知。|
|success|1|脚本成功运行。|
|失败|2|脚本无法运行。|
|scriptError|3|发现脚本命中错误。|
|pending|4 |脚本正在等待执行。|
|notApplicable|5 |脚本不适用于此设备。|




