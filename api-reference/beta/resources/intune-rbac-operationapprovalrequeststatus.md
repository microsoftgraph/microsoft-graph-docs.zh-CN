---
title: operationApprovalRequestStatus 枚举类型
description: 当前审批请求的状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b60e9071de452cdf42a8ef58246be77bdfd868a8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342235"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>operationApprovalRequestStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当前审批请求的状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知状态|
|needsApproval|1|审批请求需要经过审批，然后才能完成操作。|
|已批准|2|审批请求已批准，现在可以完成操作。|
|rejected|3|审批请求被拒绝，操作未获得批准，无法进一步操作。|
|cancelled|4|用户已取消审批请求，无需进一步操作。|
|已完成|5|审批请求已完成，无需进一步操作。|
|已过期|6 |审批请求已过期，必须进行新的审批才能完成此请求。|




