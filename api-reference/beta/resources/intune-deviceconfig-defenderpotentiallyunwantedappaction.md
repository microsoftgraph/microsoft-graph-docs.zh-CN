---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: Defender 在 PUA 中对检测到可能不需要的应用程序 (的操作) 。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 25bf816c93d48030cf1937669293f4cadf8e1c5f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797547"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 在 PUA 中对检测到可能不需要的应用程序 (的操作) 。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|PUA 保护已关闭。 Defender 不会防范可能不需要的应用程序。|
|block|1|PUA 保护已打开。 检测到的项目被阻止。 这些威胁将连同其他威胁一起显示在历史记录中。|
|audit|2|审核模式。 Defender 将检测可能不需要的应用程序，但不执行任何操作。 可以通过在事件查看器中搜索 Defender 创建的事件来查看有关 Defender 已针对的应用程序采取操作的信息。|



