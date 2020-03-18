---
title: policySetStatus 枚举类型
description: 用于指定 PolicySet 状态的枚举。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a470e6c13bfd20ada920bbe2b471bfa96379092
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775147"
---
# <a name="policysetstatus-enum-type"></a>policySetStatus 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于指定 PolicySet 状态的枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值。|
|校验|1|所有 PolicySet 项现在都在验证工作负荷的相应设置。|
|partialSuccess|双面|完成所有 PolicySet 项目的后过程，但出现故障。|
|success|第三章|部署所有 PolicySet 项目。 并不意味着所有部署都成功。 |
|error|4 |PolicySet 处理完全失败。|
|notAssigned|5 |PolicySet/PolicySetItem 未分配给任何组。|



