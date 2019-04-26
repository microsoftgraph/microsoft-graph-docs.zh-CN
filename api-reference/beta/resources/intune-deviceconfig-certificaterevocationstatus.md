---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549356"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书吊销状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未被吊销。|
|决|1|撤销挂起。|
|io|2 |已发出吊销命令。|
|未能|3 |吊销失败。|
|吊销|4 |吊销.|





