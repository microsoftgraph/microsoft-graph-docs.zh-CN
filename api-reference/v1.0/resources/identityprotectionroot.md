---
title: 标识保护 API
description: identityProtectionRoot 资源类型
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 23a356597092a6bf7f75de3cf359c2026979489b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056079"
---
# <a name="identityprotectionroot-resource-type"></a>identityProtectionRoot 资源类型

命名空间：microsoft.graph

标识保护是一种工具，允许组织发现、调查和修正其环境中基于标识的风险。 可以使用以下 Microsoft Graph API 查询 Identity Protection 检测到的风险： 

* [riskDetection](riskdetection.md) - Graph Microsoft 查询用户和登录链接风险检测的列表，以及有关检测的相关信息。 Azure AD Identity Protection 中的风险检测包括任何与目录中的用户帐户相关的已识别可疑操作。

* [riskyUsers](riskyuser.md) - 查询 Microsoft Graph，获取标识保护检测到有风险的用户的信息。 用户风险表示给定标识或帐户受到威胁的可能性。 这些风险使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构、Microsoft 的安全团队和其他受信任来源）脱机计算。

* [signIn](signin.md) - 查询 Microsoft Graph，获取与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。 登录风险表示给定身份验证请求未由标识所有者授权的概率。 可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构专业人员、Microsoft 的安全团队和其他受信任来源）实时计算或脱机计算这些风险。

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>在 Microsoft Graph 中，可以使用标识保护 API 执行哪些Graph？

以下是处理审核日志数据的常见请求：

Operation | URL
:----------|:----
获取有风险的用户 | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
获取风险检测 | [GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
获取用户的风险历史记录 | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
确认用户受到威胁 | [发布 https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
消除有风险的用户 | [发布 https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

有关特定指南和其他信息，请参阅使用 Microsoft Graph [API 识别和修正风险](/graph/tutorial-riskdetection-api)。

## <a name="what-licenses-do-i-need"></a>需要哪些许可证？

Azure AD Identity Protection 是一项高级功能。 你需要一Azure AD Premium P1或 P2 许可证才能访问 riskDetection API (注意： P1 许可证会收到有限的) 。 riskyUsers API 仅适用于Azure AD Premium P2许可证。

## <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)
* [开始使用Azure Active Directory和 Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
