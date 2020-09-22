---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb46c05ddbd1055f44794f0300077d47122aea25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081116"
---
# <a name="remediationstate-enum-type"></a>remediationState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备管理脚本的执行状态的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知结果。|
|跳过|1 |跳过了修正脚本执行|
|success|2 |已成功执行修正脚本并修正了设备状态|
|remediationFailed|第三章|已成功执行修正脚本，但未能修正设备状态|
|scriptError|4 |遇到了修正脚本执行和错误或超时|






