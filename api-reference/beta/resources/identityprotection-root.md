---
title: 使用 Azure AD 标识保护 API
description: 可以使用 Microsoft Graph查询 Identity Protection API，以接收有关 Azure AD Identity Protection 检测到的风险的信息。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 37fef748455df6511eedd631332d453a5feaaf77
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220652"
---
# <a name="use-the-azure-ad-identity-protection-api"></a>使用 Azure AD 标识保护 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

标识保护是一种工具，允许组织发现、调查和修正其环境中基于标识的风险。 可以使用以下 Microsoft Graph API 查询 Identity Protection 检测到的风险： 

* [riskDetection](riskdetection.md) - Graph Microsoft 查询用户和登录链接风险检测和与检测关联的信息的列表。 Azure AD Identity Protection 中的风险检测包括任何与目录中的用户帐户相关的已识别可疑操作。

* [riskyUsers](riskyuser.md) - 查询 Microsoft Graph，获取标识保护检测到有风险的用户的信息。 用户风险表示给定标识或帐户受到威胁的可能性。 这些风险使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构、Microsoft 的安全团队和其他受信任来源）脱机计算。

* [signIn](signin.md) - Graph Microsoft 帐户，获取与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。 登录风险表示给定身份验证请求未由标识所有者授权的概率。 可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构专业人员、Microsoft 的安全团队和其他受信任来源）实时计算或脱机计算这些风险。


>[!CAUTION]
>**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。 有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

## <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)
* [开始Azure Active Directory和 Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
