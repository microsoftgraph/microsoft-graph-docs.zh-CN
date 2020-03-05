---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc2be0c860ba142f59bba05a2a0c5ae0105c0ab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528516"
---
# <a name="remediationstate-enum-type"></a>remediationState 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知结果。|
|跳过|1 |跳过了修正脚本执行|
|success|2 |已成功执行修正脚本并修正了设备状态|
|remediationFailed|3 |已成功执行修正脚本，但未能修正设备状态|
|scriptError|4 |遇到了修正脚本执行和错误或超时|



