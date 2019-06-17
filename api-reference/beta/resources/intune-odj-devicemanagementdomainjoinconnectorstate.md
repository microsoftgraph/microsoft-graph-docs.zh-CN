---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a584a77c0a921b9d5864270c5a42a9991123eb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001914"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a>deviceManagementDomainJoinConnectorState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ODJ 请求状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|工作|0|连接器积极 ping Intune。|
|error|1|来自最近一小时内的连接器没有任何信号。|
|不再|双面|来自过去5天内的连接器没有任何信号。|





