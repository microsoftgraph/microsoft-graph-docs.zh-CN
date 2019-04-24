---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521290"
---
# <a name="managementstate-enum-type"></a>managementState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Microsoft Intune 中设备的管理状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|managed|0|设备正在管理中|
|retirePending|1|设备和 unenrolling 从管理中的过程中发生停用命令|
|retireFailed|2 |设备上的停用命令失败|
|wipePending|3 |设备和 unenrolling 中的 "擦除" 命令在管理过程中发生|
|wipeFailed|4 |设备上的擦除命令失败|
|正常|5 |设备运行不正常。|
|deletePending|6 |在设备上发生删除命令 |
|retireIssued|7 |为设备发出了停用命令|
|wipeIssued|8 |已为设备发出擦除命令|
|wipeCanceled|9 |已取消此设备的擦除命令|
|retireCanceled|10 |已取消此设备的停用命令|
|探索|11 |设备已被发现, 但未完全注册。|





