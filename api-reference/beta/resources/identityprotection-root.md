---
title: 使用 Azure AD 标识保护 Api
description: 您可以使用 Microsoft Graph 来查询标识保护 Api，以接收 Azure AD Identity Protection 检测到的风险的相关信息。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 2adaf43786f1ced76a2c971815989f08967cfb3d
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312033"
---
# <a name="use-the-azure-ad-identity-protection-api"></a>使用 Azure AD 标识保护 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

标识保护是一种工具，使组织能够在其环境中发现、调查和修正基于标识的风险。 您可以使用以下 Microsoft Graph Api 来查询由身份保护检测到的风险： 

* [riskDetection](riskdetection.md) -查询 Microsoft Graph，以获取用户和登录相关的风险检测以及有关检测的相关信息的列表。 Azure AD 标识保护中的风险检测包括与目录中的用户帐户相关的任何已确定的可疑操作。

* [riskyUsers](riskyuser.md) -查询 Microsoft Graph，以获取标识保护检测为有风险的用户的信息。 用户风险表示给定标识或帐户受到危害的可能性。 这些风险是使用 Microsoft 的内部和外部威胁智能源（包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源）进行脱机计算的。

* [登录](signin.md) 查询 Microsoft Graph，以获取有关具有与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。 登录风险表示标识所有者未授权给定的身份验证请求的可能性。 可以使用 Microsoft 的内部和外部威胁智能来源实时计算或计算这些风险，包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源。

* [identityRiskEvents](identityriskevent.md) -查询 Microsoft Graph 以获取风险检测和相关信息的列表。 此 API 已弃用;我们建议您改为使用 **riskDetections** 。

>[!CAUTION]
>**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。 有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

## <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory 标识保护](https://docs.microsoft.com/azure/active-directory/identity-protection/overview-identity-protection)
* [Azure Active Directory 标识保护和 Microsoft Graph 入门](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
