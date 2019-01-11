---
title: actionState 枚举类型
description: 在设备上的操作的状态
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0c05e283b94473a5c8c43498ff5bf1dd82da7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871937"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

在设备上的操作的状态
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|不是有效的操作状态|
|挂起|1|操作处于挂起状态|
|取消此事件|2|操作已被取消。|
|活动|3|操作处于活动状态。|
|done|4|没有错误完成的操作。|
|failed|5|失败的操作|
|notSupported|6|不支持操作。|



