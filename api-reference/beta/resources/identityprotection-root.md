---
title: 使用 Azure AD 标识保护 API (预览)
description: 您可以使用 Microsoft Graph 查询由 Azure AD Identity Protection 检测到的每种风险事件类型的 identityRiskEvent 资源。 这些事件对使用 Azure AD 高级 P2 的客户可用。 具有 Azure AD 高级 P1 的客户可以使用事件子集。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 597ff7ed156dede995b10f07ee6ac6945745b83c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506375"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>使用 Azure AD 标识保护 API (预览)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以使用 Microsoft Graph 查询由[Azure AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)检测到的每种风险事件类型的[identityRiskEvent](identityriskevent.md)资源。 这些事件对使用 Azure AD 高级 P2 的客户可用。 具有 Azure AD 高级 P1 的客户可以使用事件子集。

* [来自匿名 IP 地址的登录](anonymousipriskevent.md)
* [来自受恶意软件感染的设备的登录](malwareriskevent.md)
* [无法移动到非常规位置](impossibletravelriskevent.md)
* [凭据泄露的用户](leakedcredentialsriskevent.md)
* [来自可疑 IP 地址的登录](suspiciousipriskevent.md)
* [来自不熟悉位置的登录](unfamiliarlocationriskevent.md)

使用以下操作获取这些事件和相关信息:

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| 获取 identityRiskEvent 集合。 |
|[获取 identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| 获取 identityRiskEvent 对象。 |
|[列出 anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| 获取 anonymousIpRiskEvent 集合。 |
|[获取 anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| 获取 anonymousIpRiskEvent 对象。 |
|[列出 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| 获取 impossibleTravelRiskEvent 集合。 |
|[获取 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| 获取 impossibleTravelRiskEvent 对象。 |
|[列出 leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| 获取 leakedCredentialsRiskEvent 集合。 |
|[获取 leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| 获取 leakedCredentialsRiskEvent 对象。 |
|[列出 malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| 获取 malwareRiskEvent 集合。 |
|[获取 malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| 获取 malwareRiskEvent 对象。 |
|[列出 suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| 获取 suspiciousIpRiskEvent 集合。 |
|[获取 suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| 获取 suspiciousIpRiskEvent 对象。 |
|[列出 unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| 获取 unfamiliarLocationRiskEvent 集合。 |
|[获取 unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| 获取 unfamiliarLocationRiskEvent 对象。 |

# <a name="see-also"></a>另请参阅

* [关于 Azure Active Directory 标识保护](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Azure Active Directory 标识保护和 Microsoft Graph 入门](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprotection-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
