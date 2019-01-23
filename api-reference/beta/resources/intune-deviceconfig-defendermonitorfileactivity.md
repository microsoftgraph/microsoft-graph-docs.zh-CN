---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9b0f91d0a2d802fd573d7825da016dc8850e941
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414954"
---
# <a name="defendermonitorfileactivity-enum-type"></a>defenderMonitorFileActivity 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于监控文件活动的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|禁用|1|禁用监控文件活动。|
|monitorAllFiles|2|监视所有文件。|
|monitorIncomingFilesOnly|3| 监视传入的文件。|
|monitorOutgoingFilesOnly|4|监视传出的文件。|




