---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4849f369aa5dd04a68599050aa097b2ac63f5ef1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154780"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对检测到的恶意软件威胁执行的 Defender 的默认操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|根据更新定义应用操作。|
|clean|1|清理检测到的威胁。|
|隔离|双面|隔离检测到的威胁。|
|删除|第三章|删除检测到的威胁。|
|允许|4|允许检测到的威胁。|
|定制|5|允许用户确定要对检测到的威胁采取的操作。|
|数据|型|阻止检测到的威胁。|




