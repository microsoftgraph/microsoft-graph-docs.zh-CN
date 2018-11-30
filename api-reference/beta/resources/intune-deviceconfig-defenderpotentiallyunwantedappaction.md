---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: Defender 的操作，才能检测到可能有害的应用程序 (PUA)。
ms.openlocfilehash: c786906046d6a35c026da95246016537e4325aab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043533"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Defender 的操作，才能检测到可能有害的应用程序 (PUA)。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|PUA 保护处于关闭状态。 Defender 将不能防范可能有害的应用程序。|
|阻止|1|在 PUA 保护。 检测到的项目会被阻止。 它们将显示以及其他威胁的历史记录中。|
|审核|2|审核模式。 Defender 将检测可能有害的应用程序，但不需要任何操作。 您可以查看有关应用程序的信息 Defender 可能需要花费针对操作，通过搜索创建的 Defender 在事件查看器事件。|





