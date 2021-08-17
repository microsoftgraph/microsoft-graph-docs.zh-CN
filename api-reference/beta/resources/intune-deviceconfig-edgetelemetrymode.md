---
title: edgeTelemetryMode 枚举类型
description: 发送到分析的浏览Microsoft 365类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16efa834cf2a3a8089cd2975cb4f1c539f5114941fc307e3fe8da61dc6e390ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54142048"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

发送到分析的浏览Microsoft 365类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认 – 未收集或发送遥测数据|
|Intranet|1 |仅允许发送 Intranet 历史记录：仅发送 Intranet 网站的浏览历史记录数据|
|Internet|2 |仅允许发送 Internet 历史记录：仅发送 Internet 网站的浏览历史记录数据|
|intranetAndInternet|3 |允许发送 Intranet 和 Internet 历史记录：发送 Intranet 和 Internet 网站的浏览历史记录数据|




