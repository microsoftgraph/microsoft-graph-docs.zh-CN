---
title: enrollmentState 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3002fd793020213f8787f0c62b1e7d7c1c9ee0e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523679"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|设备注册状态未知|
|注册|1 |设备已注册。|
|pendingReset|2 |已注册，但通过注册配置文件进行了注册，并且注册的配置文件不同于分配的配置文件。|
|未能|3 |未注册，并且存在注册失败记录。|
|notContacted|4 |导入了设备，但未注册。|
|堵塞|5 |设备已注册为 userless，但由于应用程序安装失败而被阻止移到用户注册。|



