---
title: actionState 枚举类型
description: 在设备上的操作的状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421611"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




