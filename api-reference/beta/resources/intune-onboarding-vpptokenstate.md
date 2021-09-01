---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c7addece5e6cf2281e99439c957ceb567a28de73
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790610"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple Volume Purchase Program 令牌关联的可能状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|valid|1|令牌有效。|
|已过期|2|令牌已过期。|
|无效|3|令牌无效。|
|assignedToExternalMDM|4 |令牌由另一个 MDM 服务管理。|
|duplicateLocationId|5 |令牌与帐户上另一个令牌的相同位置相关联。|



