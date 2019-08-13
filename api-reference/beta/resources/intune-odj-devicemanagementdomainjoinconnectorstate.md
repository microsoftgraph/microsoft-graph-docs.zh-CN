---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f664a6b57d92f5a8cd2d586f8bc2747ffa6db71c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342003"
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



