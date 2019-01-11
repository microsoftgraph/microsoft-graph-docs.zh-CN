---
title: enrollmentState 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a3790733067598442af615cb90b8ae347fd228
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869018"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|unknown|0|设备注册状态是未知|
|注册|1|注册设备。|
|pendingReset|2|注册但它通过注册配置文件中注册的注册的配置文件是不同的已分配的配置文件。|
|failed|3|未注册，并且没有注册失败记录。|
|notContacted|4|导入但未注册设备。|
|已阻止|5|设备注册为 userless，但阻止移动到用户注册，因为应用程序安装失败。|





