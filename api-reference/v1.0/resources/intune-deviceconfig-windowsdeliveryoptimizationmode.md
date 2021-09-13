---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c720a9208f948e8a594b42df00119e5f3e45ded0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055959"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对等分发的传递优化模式

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|httpOnly|1|仅 HTTP，无对等|
|httpWithPeeringNat|2|操作系统默认值 – Http 与同一网络地址转换器后的对等混合|
|httpWithPeeringPrivateGroup|3|通过专用组对等混合的 HTTP|
|httpWithInternetPeering|4 |HTTP 与 Internet 对等混合|
|simpleDownload|99|无对等的简单下载模式|
|bypassMode|100|绕过模式。 请勿使用传递优化并改为使用 BITS|




