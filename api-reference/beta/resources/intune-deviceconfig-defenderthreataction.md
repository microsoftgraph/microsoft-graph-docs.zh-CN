---
title: defenderThreatAction 枚举类型
description: Defender 的默认操作以对其执行检测到恶意软件的威胁。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400268"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 的默认操作以对其执行检测到恶意软件的威胁。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|应用基于更新定义的操作。|
|clean|1|清理检测到的威胁。|
|隔离|2|隔离检测到的威胁。|
|删除|3|删除检测到的威胁。|
|允许|4|允许检测到的威胁。|
|用户定制|5|允许用户以确定要使用的检测威胁采取的操作。|
|阻止|6|阻止检测到的威胁。|




