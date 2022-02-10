---
title: 使用 Microsoft Graph标识保护 API
description: 使用 Microsoft Graph查询和接收有关 Identity Protection 检测到Azure AD的信息。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 7a32a563c2b918c68a7cd14e2627c80bffba7976
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519514"
---
# <a name="use-the-microsoft-graph-identity-protection-apis"></a>使用 Microsoft Graph标识保护 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) 是一种工具，允许组织发现、调查和修正其组织中基于标识Azure AD风险。 

使用以下 Microsoft Graph API 查询 Identity Protection 检测到的用户和服务Azure AD风险：

## <a name="for-users"></a>对于用户

+ [riskDetection](riskdetection.md) - Graph Microsoft 查询用户和登录链接风险检测的列表，以及有关检测的相关信息。 Identity Protection 中Azure AD检测包括任何与目录中的用户帐户相关的已识别可疑操作。

    >[!CAUTION]
    >**identityRiskEvents** API 已弃用，在 2020 年 1 月 10 日停止返回数据。 它已被 [riskDetection](riskdetection.md) API 取代。 有关弃用的信息，请参阅弃 [用 identityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

+ [riskyUsers](riskyuser.md) - 查询 Microsoft Graph，了解标识保护Azure AD有风险的用户的信息。 用户风险表示给定标识或帐户受到威胁的可能性。 这些风险使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构、Microsoft 的安全团队和其他受信任来源）脱机计算。

+ [signIn](signin.md) - Graph Microsoft Azure AD使用与风险状态、详细信息和级别相关的特定属性登录的信息。 登录风险表示给定身份验证请求未由标识所有者授权的概率。 可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构专业人员、Microsoft 的安全团队和其他受信任来源）实时或脱机计算这些风险。

## <a name="for-service-principals"></a>对于服务主体

+ [servicePrincipalRiskDetection](serviceprincipalriskdetection.md) - 向 Microsoft Graph查询服务主体风险检测和与检测关联的信息的列表。 Identity Protection 中Azure AD检测包括任何与目录中的服务主体帐户相关的已识别可疑操作。

+ [riskyServicePrincipals](riskyserviceprincipal.md) - 向 Microsoft Graph查询有关 Identity Protection 检测到Azure AD存在风险的服务主体的信息。 服务主体风险表示给定标识或帐户受到威胁的可能性。 这些风险使用来自 Microsoft 内部和外部威胁情报源（包括安全研究人员、执法机构专业人员、Microsoft 安全团队和其他受信任来源）的数据和模式异步计算。

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>Microsoft Graph 中的标识保护 API 可以Graph？

以下是热门请求：

操作 | URL
:----------|:----
获取有风险的用户 | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=beta)
获取风险检测 | [GET https://graph.microsoft.com/beta/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=beta)
获取用户的风险历史记录 | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=beta)
确认用户受到威胁 | [发布 https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=beta)
消除有风险的用户 | [发布 https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=beta)

有关特定指南和其他信息，请参阅使用 [Microsoft Graph API 识别和修正风险](/graph/tutorial-riskdetection-api)。

## <a name="what-licenses-do-i-need"></a>需要哪些许可证？

Azure AD Identity Protection 是一项高级功能。 你需要一个 Azure AD Premium P1 或 P2 许可证才能访问 Microsoft Graph [riskDetection API](riskdetection.md) (注意： P1 许可证会收到有限的) 。 [riskyUsers API](riskyuser.md) 仅适用于Azure AD Premium P2许可证。

## <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)
* [开始使用 Azure Active Directory Identity Protection 和 Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
