---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eabc09c8eba7267041eaf5bb318d6269373f48b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091549"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对等分发的传递优化模式

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|允许用户进行设置。|
|httpOnly|1 |仅限 HTTP，无对等|
|httpWithPeeringNat|2 |OS 默认值–在同一网络地址转换器后具有对等的 Http 混合|
|httpWithPeeringPrivateGroup|第三章|通过专用组与对等互连的 HTTP 混合|
|httpWithInternetPeering|4 |与 Internet 对等混合的 HTTP|
|simpleDownload|99|无对等的简单下载模式|
|bypassMode|100|旁路模式。 请勿使用传递优化和改用 BITS|









