---
title: 使用 Azure AD 身份保护 API （预览）
description: 您可以使用 Microsoft Graph 查询每种类型的风险事件检测到的 Azure AD 身份保护 identityRiskEvent 资源。 这些事件可供客户与 Azure AD Premium P2。 适用于与 Azure AD Premium P1 客户事件的子集。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 9c92be83fd3248ad10578446f91b38176913da1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953621"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>使用 Azure AD 身份保护 API （预览）

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以使用 Microsoft Graph 查询每种类型的风险事件检测到的[Azure AD 身份保护](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection) [identityRiskEvent](identityriskevent.md)资源。 这些事件可供客户与 Azure AD Premium P2。 适用于与 Azure AD Premium P1 客户事件的子集。

* [从匿名登录 IP 地址](anonymousipriskevent.md)
* [从感染恶意软件的设备登录](malwareriskevent.md)
* [对在典型的位置的意思出差](impossibletravelriskevent.md)
* [具有泄漏凭据的用户](leakedcredentialsriskevent.md)
* [登录从可疑 IP 地址](suspiciousipriskevent.md)
* [从不熟悉位置登录](unfamiliarlocationriskevent.md)

使用以下操作来获取这些事件和关联的信息：

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| 获取 identityRiskEvent 集合。 |
|[获取 identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| 获取 identityRiskEvent 对象。 |
|[列表 anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| 获取 anonymousIpRiskEvent 集合。 |
|[获取 anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| 获取 anonymousIpRiskEvent 对象。 |
|[列表 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| 获取 impossibleTravelRiskEvent 集合。 |
|[获取 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| 获取 impossibleTravelRiskEvent 对象。 |
|[列表 leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| 获取 leakedCredentialsRiskEvent 集合。 |
|[获取 leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| 获取 leakedCredentialsRiskEvent 对象。 |
|[列表 malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| 获取 malwareRiskEvent 集合。 |
|[获取 malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| 获取 malwareRiskEvent 对象。 |
|[列表 suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| 获取 suspiciousIpRiskEvent 集合。 |
|[获取 suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| 获取 suspiciousIpRiskEvent 对象。 |
|[列表 unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| 获取 unfamiliarLocationRiskEvent 集合。 |
|[获取 unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| 获取 unfamiliarLocationRiskEvent 对象。 |

# <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory 标识保护](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Azure Active Directory 身份防护和 Microsoft Graph 入门](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
