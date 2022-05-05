---
title: operationApprovalRequestStatus 枚举类型
description: 当前审批请求的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0068b5805ec8668e75a470b6d94ca16cdab2ca0e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210736"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>operationApprovalRequestStatus 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当前审批请求的状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知状态|
|needsApproval|1|审批请求需要审批才能完成操作。|
|批准|2|批准请求已批准，现在可以完成操作。|
|拒绝|3|审批请求被拒绝，操作未获批准，无法采取进一步操作。|
|取消|4|用户取消了审批请求，无需采取进一步操作。|
|完成|5|审批请求已完成，无需采取进一步操作。|
|过期|6 |审批请求已过期，必须进行新的审批才能完成此请求。|
|unknownFutureValue|99|未来操作审批请求状态的占位符。|




