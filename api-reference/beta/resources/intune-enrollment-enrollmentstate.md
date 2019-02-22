---
title: enrollmentState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcb039563d9c45a33c4e42344fc8557dfe29b333
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159246"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|设备注册状态未知|
|注册|1|设备已注册。|
|pendingReset|双面|已注册, 但通过注册配置文件进行了注册, 并且注册的配置文件不同于分配的配置文件。|
|failed|第三章|未注册, 并且存在注册失败记录。|
|notContacted|4|导入了设备, 但未注册。|
|已阻止|5|设备已注册为 userless, 但由于应用程序安装失败而被阻止移到用户注册。|




