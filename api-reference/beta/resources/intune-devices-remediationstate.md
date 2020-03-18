---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd940bbe2256baa7954e67ba9469ac00740f4ad1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783912"
---
# <a name="remediationstate-enum-type"></a>remediationState 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知结果。|
|跳过|1|跳过了修正脚本执行|
|success|双面|已成功执行修正脚本并修正了设备状态|
|remediationFailed|第三章|已成功执行修正脚本，但未能修正设备状态|
|scriptError|4 |遇到了修正脚本执行和错误或超时|



