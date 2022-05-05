---
title: zebraFotaConnectorState 枚举类型
description: 表示 Zebra FOTA 连接器的各种状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d7d5e8dfd7413b43f7ac1835c7b4ce07c92480f9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213142"
---
# <a name="zebrafotaconnectorstate-enum-type"></a>zebraFotaConnectorState 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Zebra FOTA 连接器的各种状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|尚未设置连接器 (尚未使用该功能的默认值) 。|
|连接|1|连接状态指示Intune已链接到当前租户的 Zebra 更新服务。|
|断开|2|断开连接状态指示帐户在过去和之后已连接。|
|unknownFutureValue|99|未知的未来枚举值。|




