---
title: defenderThreatAction 枚举类型
description: 要对检测到的恶意软件威胁执行的 Defender 的默认操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 472670b58115d9887ae44a2fb191f1338d058fb4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269362"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对检测到的恶意软件威胁执行的 Defender 的默认操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|根据更新定义应用操作。|
|清理|1|清理检测到的威胁。|
|隔离|双面|隔离检测到的威胁。|
|删除|第三章|删除检测到的威胁。|
|允许|4 |允许检测到的威胁。|
|定制|5 |允许用户确定要对检测到的威胁采取的操作。|
|数据|6 |阻止检测到的威胁。|




