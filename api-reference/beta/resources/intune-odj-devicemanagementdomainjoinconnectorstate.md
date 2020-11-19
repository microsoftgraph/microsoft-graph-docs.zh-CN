---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 58b0a3a9e590913d0415062d6737fc6d9c33c451
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222756"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a>deviceManagementDomainJoinConnectorState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ODJ 请求状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|工作|0|连接器积极 ping Intune。|
|error|1|来自最近一小时内的连接器没有任何信号。|
|不再|双面|来自过去5天内的连接器没有任何信号。|




