---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c53847d270639d11b5014291e62dde2668a4d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534379"
---
# <a name="defendermonitorfileactivity-enum-type"></a>defenderMonitorFileActivity 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

监视文件活动的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义, 默认值, 无意向。|
|disable|1|禁用监控文件活动。|
|monitorAllFiles|2 |监视所有文件。|
|monitorIncomingFilesOnly|3 | 仅监视传入的文件。|
|monitorOutgoingFilesOnly|4 |仅监视传出文件。|



