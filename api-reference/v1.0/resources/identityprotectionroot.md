---
title: 标识保护 Api
description: identityProtectionRoot 资源类型
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d7b31b0a27ca96333087d55b3666f97eefdd70b9
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898049"
---
# <a name="identityprotectionroot-resource-type"></a>identityProtectionRoot 资源类型

命名空间：microsoft.graph

标识保护是一种工具，使组织能够在其环境中发现、调查和修正基于标识的风险。 您可以使用以下 Microsoft Graph Api 来查询由身份保护检测到的风险： 

* [riskDetection](riskdetection.md) -查询 Microsoft Graph，以获取用户和登录相关的风险检测以及有关检测的相关信息的列表。 Azure AD 标识保护中的风险检测包括与目录中的用户帐户相关的任何已确定的可疑操作。

* [riskyUsers](riskyuser.md) -查询 Microsoft Graph，以获取标识保护检测为有风险的用户的信息。 用户风险表示给定标识或帐户受到危害的可能性。 这些风险是使用 Microsoft 的内部和外部威胁智能源（包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源）进行脱机计算的。

* [登录](signin.md)查询 Microsoft Graph，以获取有关具有与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。 登录风险表示标识所有者未授权给定的身份验证请求的可能性。 可以使用 Microsoft 的内部和外部威胁智能来源实时计算或计算这些风险，包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源。

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>在 Microsoft Graph 中，我可以对身份保护 Api 执行哪些操作？

以下是处理审核日志数据的常见请求：

Operation | URL
:----------|:----
获取有风险的用户 | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUser](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
获取风险检测 | [GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
获取用户的风险历史记录 | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
确认用户是否受到威胁 | [发布https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
消除有风险的用户 | [发布https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

## <a name="what-licenses-do-i-need"></a>需要哪些许可证？

Azure AD Identity Protection 是一项高级功能。 您需要使用 Azure AD 高级 P1 或 P2 许可证来访问 riskDetection API （注意： P1 许可证收到有限的风险信息）。 RiskyUsers API 仅适用于 Azure AD Premium P2 许可证。

## <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory 标识保护](https://docs.microsoft.com/azure/active-directory/identity-protection/overview-identity-protection)
* [Azure Active Directory 标识保护和 Microsoft Graph 入门](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-identity-protection-graph-api)


