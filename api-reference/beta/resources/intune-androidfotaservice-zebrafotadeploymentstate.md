---
title: zebraFotaDeploymentState 枚举类型
description: 表示 Zebra FOTA 部署的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5912f89249951db9ff4dd5a058169cb3b54113fc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213182"
---
# <a name="zebrafotadeploymentstate-enum-type"></a>zebraFotaDeploymentState 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Zebra FOTA 部署的状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|pendingCreation|0|部署已创建，但 Zebra 尚未确认其创建。|
|createFailed|1|部署未使用 Zebra 成功创建。|
|已创建|2|部署已创建，但尚未部署。|
|inProgress|3|部署已开始但尚未完成。|
|完成|4|部署已完成或结束日期已过。|
|pendingCancel|5|管理员已请求取消部署，但 Zebra 尚未确认取消。|
|取消|6 |Zebra 已成功取消部署。|
|unknownFutureValue|99|未知的未来枚举值。|




