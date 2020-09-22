---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: 要对检测到的可能有害的应用程序 (PUA) 执行的 Defender 操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff44e62d67a5acde9a87e1238b72caed29677452
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089523"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对检测到的可能有害的应用程序 (PUA) 执行的 Defender 操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|PUA 保护已关闭。 Defender 将无法抵御可能有害的应用程序。|
|数据|1 |PUA 保护已开启。 已检测到的项目被阻止。 它们将显示在历史记录中，以及其他威胁。|
|跟踪|2 |审核模式。 Defender 将检测可能有害的应用程序，但不执行任何操作。 您可以通过在事件查看器中搜索由 Defender 创建的事件，查看有关应用程序 Defender 执行操作的相关信息。|






