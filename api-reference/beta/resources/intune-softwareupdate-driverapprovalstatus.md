---
title: driverApprovalStatus 枚举类型
description: 表示驱动程序的审批状态的枚举类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dbf9f081ea77e872cf99e3d2f28b829c3935b5e7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793686"
---
# <a name="driverapprovalstatus-enum-type"></a>driverApprovalStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示驱动程序的审批状态的枚举类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|needsReview|0|这表示驱动程序需要 IT 管理员审查。|
|declined|1|这表示 IT 管理员已拒绝驱动程序。|
|已批准|2|这表示 IT 管理员已批准驱动程序。|
|已挂起|3|这表示 IT 管理员已暂停驱动程序。|



