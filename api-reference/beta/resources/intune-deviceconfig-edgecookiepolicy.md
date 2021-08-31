---
title: edgeCookiePolicy 枚举类型
description: 用于指定允许哪些 cookie 在缓存中Microsoft Edge。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 66fd6faa5db131052bcc63dbb9565de03ea45a4e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796872"
---
# <a name="edgecookiepolicy-enum-type"></a>edgeCookiePolicy 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于指定允许哪些 cookie 在缓存中Microsoft Edge。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|allow|1|允许。|
|blockThirdParty|2|仅阻止第三方 Cookie。|
|blockAll|3|阻止所有 Cookie。|



