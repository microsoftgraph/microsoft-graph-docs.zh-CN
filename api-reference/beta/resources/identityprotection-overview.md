---
title: 使用 Microsoft Graph标识保护 API
description: 使用 Microsoft Graph查询和接收有关Azure AD标识保护检测到的风险的信息。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 07ca6a9d6b50cd702d7ea1543a5fd07d8f8ff376
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061123"
---
# <a name="use-the-microsoft-graph-identity-protection-apis"></a>使用 Microsoft Graph标识保护 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) [标识保护](/azure/active-directory/identity-protection/overview-identity-protection)是允许组织发现、调查和修正其Azure AD组织中基于标识的风险的工具。

使用以下 Microsoft Graph API 查询Azure AD标识保护检测到的用户和服务主体风险：

## <a name="for-users"></a>对于用户

+ [riskDetection](riskdetection.md) - 查询 Microsoft Graph，以获取用户和登录链接风险检测的列表以及有关检测的相关信息。 Azure AD标识保护中的风险检测包括与目录中的用户帐户相关的任何已识别的可疑操作。

    >[!CAUTION]
    >**identityRiskEvents** API 已弃用，并在 2020 年 1 月 10 日停止返回数据。 它已替换为 [riskDetection](riskdetection.md) API。 有关弃用的详细信息，请参阅 [IdentityRiskEvents API 的弃](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)用。

+ [riskyUsers](riskyuser.md) - 查询 Microsoft Graph，以获取有关Azure AD标识保护检测为有风险的用户的信息。 用户风险表示给定标识或帐户遭到入侵的概率。 这些风险是使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法专业人员、Microsoft 安全团队和其他受信任来源）脱机计算的。

+ [signIn](signin.md) - 查询 Microsoft Graph，以获取与风险状态、详细信息和级别相关的特定属性Azure AD登录的信息。 登录风险表示标识所有者未授权给定身份验证请求的概率。 这些风险可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法专业人员、Microsoft 的安全团队和其他受信任的来源）实时计算或脱机计算。

## <a name="for-service-principals"></a>对于服务主体

+ [servicePrincipalRiskDetection](serviceprincipalriskdetection.md) - 查询 Microsoft Graph，以获取服务主体风险检测列表和有关检测的相关信息。 Azure AD标识保护中的风险检测包括与目录中的服务主体帐户相关的任何已识别的可疑操作。

+ [riskyServicePrincipals](riskyserviceprincipal.md) - 查询 Microsoft Graph，以获取有关Azure AD标识保护检测为有风险的服务主体的信息。 服务主体风险表示给定标识或帐户遭到入侵的概率。 这些风险是使用来自 Microsoft 内部和外部威胁情报源的数据和模式异步计算的，其中包括安全研究人员、执法专业人员、Microsoft 安全团队和其他受信任的来源。

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>如何在 Microsoft Graph 中使用标识保护 API？

以下是常用请求：

操作 | URL
:----------|:----
获取有风险的用户 | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=beta)
GET 风险检测 | [GET https://graph.microsoft.com/beta/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=beta)
获取用户的风险历史记录 | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=beta)
确认用户已泄露 | [发布 https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=beta)
消除有风险的用户 | [发布 https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=beta)

有关具体指南和其他信息，请参阅[使用 Microsoft Graph API 识别和修正风险](/graph/tutorial-riskdetection-api)。

## <a name="what-licenses-do-i-need"></a>需要哪些许可证？

Azure AD标识保护是一项高级功能。 需要一个Azure AD Premium P1或 P2 许可证才能访问 Microsoft Graph [riskDetection API](riskdetection.md) (注意：P1 许可证) 收到有限的风险信息。 [riskyUsers API](riskyuser.md) 仅适用于Azure AD Premium P2许可证。

## <a name="how-much-data-is-available"></a>有多少数据可用？

风险数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的约束。


## <a name="see-also"></a>另请参阅

* [关于Azure Active Directory标识保护](/azure/active-directory/identity-protection/overview-identity-protection)
* [使用 Azure Active Directory 标识保护和 Microsoft Graph 开始](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
