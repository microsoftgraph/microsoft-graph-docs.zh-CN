---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251501"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对等分发的传递优化模式

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|httpOnly|1|仅限 HTTP, 无对等|
|httpWithPeeringNat|双面|OS 默认值–在同一网络地址转换器后具有对等的 Http 混合|
|httpWithPeeringPrivateGroup|第三章|通过专用组与对等互连的 HTTP 混合|
|httpWithInternetPeering|4|与 Internet 对等混合的 HTTP|
|simpleDownload|99|无对等的简单下载模式|
|bypassMode|100|旁路模式。 请勿使用传递优化和改用 BITS|



