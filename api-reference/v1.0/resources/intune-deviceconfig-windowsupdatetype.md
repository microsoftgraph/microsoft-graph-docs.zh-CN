---
title: windowsUpdateType 枚举类型
description: 分支的设备将接收从其更新
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 198b5f8db5698d309199964e4cb69f8981ceeb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838967"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

分支的设备将接收从其更新
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|用户定制|0|允许用户设置。|
|all|1|半年 （目标） 通道。 设备从半年通道 （目标） 中获取所有适用的功能更新。|
|businessReadyOnly|2|半年通道。 设备获取更新功能从半年通道。|
|windowsInsiderBuildFast|3|Windows 内幕生成-Fast|
|windowsInsiderBuildSlow|4|Windows 内幕生成-速度较慢|
|windowsInsiderBuildRelease|5|Windows 内幕发布版本|



