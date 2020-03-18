---
title: actionState 枚举类型
description: 设备上操作的状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 734fa5b7920c64ed2f649f78a2e81de068e3e0db
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772256"
---
# <a name="actionstate-enum-type"></a>actionState 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备上操作的状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|操作状态无效|
|决|1|操作挂起|
|取消|双面|操作已被取消。|
|工作|第三章|操作处于活动状态。|
|done|4 |操作已完成，无错误。|
|未能|5 |操作失败|
|notSupported|6 |操作不受支持。|



