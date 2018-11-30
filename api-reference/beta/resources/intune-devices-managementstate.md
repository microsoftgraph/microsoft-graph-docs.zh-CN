---
title: 管理枚举类型
description: 管理 Microsoft Intune 中设备的状态。
ms.openlocfilehash: 554e06ff32102285d4851a19350c7c44d11d1fb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047549"
---
# <a name="managementstate-enum-type"></a>管理枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理 Microsoft Intune 中设备的状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|托管|0|在管理下的设备位于|
|retirePending|1|废弃命令正在撤消设备上并且正在 unenrolling 从管理|
|retireFailed|2|停用命令在设备上失败|
|wipePending|3|擦除命令正在撤消设备上并且正在 unenrolling 从管理|
|wipeFailed|4|擦除设备上失败的命令|
|不正常|5|设备不正常。|
|deletePending|6|删除命令正在撤消对设备 |
|retireIssued|7|为设备发出了废弃命令|
|wipeIssued|8|为设备发出了擦除命令|
|wipeCanceled|9|此设备擦除命令已被取消|
|retireCanceled|10|此设备废弃命令已被取消|
|发现|11|发现但不是完全注册的设备。|





