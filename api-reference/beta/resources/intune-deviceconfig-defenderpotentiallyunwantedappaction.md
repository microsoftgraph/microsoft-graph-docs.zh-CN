---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: Defender 的操作，才能检测到可能有害的应用程序 (PUA)。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422752"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 的操作，才能检测到可能有害的应用程序 (PUA)。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|PUA 保护处于关闭状态。 Defender 将不能防范可能有害的应用程序。|
|阻止|1|在 PUA 保护。 检测到的项目会被阻止。 它们将显示以及其他威胁的历史记录中。|
|审核|2|审核模式。 Defender 将检测可能有害的应用程序，但不需要任何操作。 您可以查看有关应用程序的信息 Defender 可能需要花费针对操作，通过搜索创建的 Defender 在事件查看器事件。|




