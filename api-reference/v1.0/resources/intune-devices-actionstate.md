---
title: actionState 枚举类型
description: 设备上操作的状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e11fc186dcfe16005e3ceaab5c6306f5893a8598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418165"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

命名空间： microsoft. graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备上操作的状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|操作状态无效|
|决|1 |操作挂起|
|取消|2 |操作已被取消。|
|工作|3 |操作处于活动状态。|
|done|4 |操作已完成，无错误。|
|未能|5 |操作失败|
|notSupported|6 |操作不受支持。|




