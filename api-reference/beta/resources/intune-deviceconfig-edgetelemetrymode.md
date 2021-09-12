---
title: edgeTelemetryMode 枚举类型
description: 发送到分析的浏览Microsoft 365类型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0e81e7ccb58db94851e2c56b269dc25050a8c35d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009173"
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
|Intranet|1|仅允许发送 Intranet 历史记录：仅发送 Intranet 网站的浏览历史记录数据|
|Internet|2|仅允许发送 Internet 历史记录：仅发送 Internet 网站的浏览历史记录数据|
|intranetAndInternet|3|允许发送 Intranet 和 Internet 历史记录：发送 Intranet 和 Internet 网站的浏览历史记录数据|



