---
title: actionState 枚举类型
description: 在设备上的操作的状态
ms.openlocfilehash: 1a18eb87cb4c9162777d16dc866de5f5766c87b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011150"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

在设备上的操作的状态
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|不是有效的操作状态|
|挂起|1|操作处于挂起状态|
|取消此事件|2|操作已被取消。|
|活动|3|操作处于活动状态。|
|done|4|没有错误完成的操作。|
|failed|5|失败的操作|
|notSupported|6|不支持操作。|



