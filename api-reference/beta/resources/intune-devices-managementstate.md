---
title: 管理枚举类型
description: 管理 Microsoft Intune 中设备的状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420015"
---
# <a name="managementstate-enum-type"></a>管理枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




