---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a2e05fe9c378f14f1b60a0ac520301010c5ac5c
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730663"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对等分发的传递优化模式

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|httpOnly|1|仅 HTTP，无对等互连|
|httpWithPeeringNat|2|OS 默认值 - Http 与同一网络地址翻译器后面的对等互连混合|
|httpWithPeeringPrivateGroup|3|跨专用组与对等互连混合的 HTTP|
|httpWithInternetPeering|4|与 Internet 对等互连混合的 HTTP|
|simpleDownload|99|无对等互连的简单下载模式|
|bypassMode|100|绕过模式。 请勿改用传递优化和使用 BITS|





