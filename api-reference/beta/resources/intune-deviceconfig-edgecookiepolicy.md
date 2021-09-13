---
title: edgeCookiePolicy 枚举类型
description: 可能的值，用于指定允许哪些 cookie 在Microsoft Edge。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 53b883efb2d09182a5ae99cc1a4e5beb74e41e1b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075548"
---
# <a name="edgecookiepolicy-enum-type"></a>edgeCookiePolicy 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

可能的值，用于指定允许哪些 cookie 在Microsoft Edge。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|允许用户设置。|
|allow|1|允许。|
|blockThirdParty|2|仅阻止第三方 Cookie。|
|blockAll|3|阻止所有 Cookie。|



