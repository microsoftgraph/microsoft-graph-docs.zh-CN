---
title: defenderThreatAction 枚举类型
description: Defender 针对检测到的恶意软件威胁执行的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 18e8fe9b691e69cf63652dae9d7e8647694f1db9
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734331"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 针对检测到的恶意软件威胁执行的默认操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|根据更新定义应用操作。|
|清洁|1|清除检测到的威胁。|
|隔离|2|隔离检测到的威胁。|
|删除|3|删除检测到的威胁。|
|允许|4|允许检测到的威胁。|
|userDefined|5|允许用户确定要对检测到的威胁执行的操作。|
|块|6 |阻止检测到的威胁。|





