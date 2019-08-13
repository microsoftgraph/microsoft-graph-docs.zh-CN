---
title: edgeTelemetryMode 枚举类型
description: 发送到 Microsoft 365 analytics 的浏览数据的类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fa6ea5a2bf187a753705b369f3f8a2558860c3eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357269"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

发送到 Microsoft 365 analytics 的浏览数据的类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值–没有收集或发送的遥测数据|
|在内|1|仅允许发送 intranet 历史记录: 仅发送 intranet 网站的浏览历史记录数据|
|访问|双面|仅允许发送 internet 历史记录: 仅发送 internet 网站的浏览历史记录数据|
|intranetAndInternet|第三章|允许同时发送 intranet 和 internet 历史记录: 为 intranet 和 internet 站点发送浏览历史记录数据|



