---
title: configurationManagerActionType 枚举类型
description: Configuration Manager 客户端上的操作类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6884ebcbe4e8c4c4b6f7b6cd6fc23246875ca7bf
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711905"
---
# <a name="configurationmanageractiontype-enum-type"></a>configurationManagerActionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Configuration Manager 客户端上的操作类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|refreshMachinePolicy|0|在 Configuration Manager 客户端上刷新计算机策略|
|refreshUserPolicy|1|在 Configuration Manager 客户端上刷新用户策略|
|wakeUpClient|2|唤醒 Configuration Manager 客户端|
|appEvaluation|3|Configuration Manager 客户端上的评估应用程序策略|
|quickScan|5|Configuration Manager 客户端上的评估应用程序策略|
|fullScan|6 |Configuration Manager 客户端上的评估应用程序策略|
|windowsDefenderUpdateSignatures|7 |Configuration Manager 客户端上的评估应用程序策略|




