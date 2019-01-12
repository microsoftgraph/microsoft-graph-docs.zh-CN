---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b0048385930166de3329ef9d407f5ddd19efc77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911894"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备注册状态。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notRegistered|0|未注册设备。|
|注册|2|已注册设备。|
|吊销|3|已阻止、 擦除或停用该设备。|
|keyConflict|4|设备具有键冲突。|
|approvalPending|5|设备是待审批状态。|
|certificateReset|6|设备证书已被重置。|
|notRegisteredPendingEnrollment|7|未注册设备以及待处理的注册。|
|unknown|8|未知设备注册状态。|



