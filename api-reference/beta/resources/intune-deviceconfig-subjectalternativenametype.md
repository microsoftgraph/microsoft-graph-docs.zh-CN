---
title: subjectAlternativeNameType 枚举类型
description: 使用者替代名称选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 812aacf65bc73aade6eafc441fafda914ea6a3b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423298"
---
# <a name="subjectalternativenametype-enum-type"></a>subjectAlternativeNameType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

使用者替代名称选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|没有使用者替代名称。|
|emailAddress|1|电子邮件地址。|
|userPrincipalName|2|用户主体名称 (UPN)。|
|customAzureADAttribute|4|自定义的 Azure AD 属性。|
|domainNameService|8|域名服务 (DNS)。|




