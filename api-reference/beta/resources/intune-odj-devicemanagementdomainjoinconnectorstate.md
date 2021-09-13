---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cb637b2ee8d720859169dd10462334dde794de54
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017252"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a>deviceManagementDomainJoinConnectorState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ODJ 请求状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|active|0|连接器正在主动 ping Intune。|
|error|1|连接器从过去一小时内没有心跳。|
|inactive|2|连接器最近 5 天没有心跳。|



