---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a53906018d45181bd16750e4ed3f0dac9dcb0d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398812"
---
# <a name="vpptokensyncstatus-enum-type"></a>vppTokenSyncStatus 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

使用 Apple 卷购买计划令牌关联的可能的同步状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|默认状态。|
|正在进行|1|正在进行的上次同步。|
|完成|2|上次同步已成功完成。|
|failed|3|上次同步失败。|




