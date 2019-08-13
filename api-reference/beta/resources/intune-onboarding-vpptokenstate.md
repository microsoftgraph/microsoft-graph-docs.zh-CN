---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d0c5db4ffaac3a08edad42e7529b62337bf0ed52
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369358"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple Volume Purchase Program 令牌关联的可能状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|有效|1|令牌有效。|
|期满|双面|令牌已过期。|
|无效|第三章|令牌无效。|
|assignedToExternalMDM|4|令牌由另一个 MDM 服务管理。|



