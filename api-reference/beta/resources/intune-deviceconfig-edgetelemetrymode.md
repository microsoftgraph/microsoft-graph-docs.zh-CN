---
title: edgeTelemetryMode 枚举类型
description: 浏览数据发送到 Microsoft 365 分析的类型
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429444"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

浏览数据发送到 Microsoft 365 分析的类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值 – 没有遥测数据收集或发送|
|intranet|1|允许发送 intranet 历史记录： 仅发送浏览 intranet 网站的历史记录数据|
|internet|2|允许发送 internet 历史记录： 仅发送浏览的 internet 站点的历史记录数据|
|intranetAndInternet|3|允许发送 intranet 和 internet 历史记录： 发送浏览 intranet 和 internet 网站的历史记录数据|




