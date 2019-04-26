---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554147"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对等分发的传递优化模式

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|httpOnly|1|仅限 HTTP, 无对等|
|httpWithPeeringNat|2 |OS 默认值–在同一网络地址转换器后具有对等的 Http 混合|
|httpWithPeeringPrivateGroup|3 |通过专用组与对等互连的 HTTP 混合|
|httpWithInternetPeering|4 |与 Internet 对等混合的 HTTP|
|simpleDownload|99|无对等的简单下载模式|
|bypassMode|100|旁路模式。 请勿使用传递优化和改用 BITS|





