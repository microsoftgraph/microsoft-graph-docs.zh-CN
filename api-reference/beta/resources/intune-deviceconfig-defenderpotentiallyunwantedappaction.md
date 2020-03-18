---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: 要对检测到的可能有害的应用程序（PUA）执行的 Defender 操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0c99cf04b217239fb1a06b2a6c26dcacc6c61cf7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794464"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对检测到的可能有害的应用程序（PUA）执行的 Defender 操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|PUA 保护已关闭。 Defender 将无法抵御可能有害的应用程序。|
|数据|1|PUA 保护已开启。 已检测到的项目被阻止。 它们将显示在历史记录中，以及其他威胁。|
|跟踪|双面|审核模式。 Defender 将检测可能有害的应用程序，但不执行任何操作。 您可以通过在事件查看器中搜索由 Defender 创建的事件，查看有关应用程序 Defender 执行操作的相关信息。|



