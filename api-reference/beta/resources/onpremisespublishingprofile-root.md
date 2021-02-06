---
title: 本地发布配置文件
description: 各种 Azure (例如，Azure Active Directory Connect Passthrough Authentication、Workday 到预配) 的 Azure AD 用户允许从企业网络外部对各种本地资源进行条件访问。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 44d09da274413b23092afea6290c0c32a64f8500
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134874"
---
# <a name="on-premises-publishing-profiles"></a>本地发布配置文件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure (例如，Azure Active Directory Connect [Passthrough](/azure/active-directory/hybrid/how-to-connect-pta)Authentication、Workday [to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial)和应用程序 [代理](https://aka.ms/whyappproxy)  允许从企业网络外部访问各种本地资源。 [可以将租户](onpremisesagent.md) (安装的应用程序代理或) 连接器[](connector.md)配置为将请求路由到特定的[已发布资源](publishedresource.md)。
[通过应用程序](onpremisesagentgroup.md) (代理) 代理组[](connectorgroup.md)或连接器组，租户管理员能够分配特定代理，为发布的特定本地资源提供服务。 租户管理员可以将多个代理组合在一起，然后将每个已发布的资源分配给一个组。 同一本地发布类型的整个实体集由 [onPremisesPublishingProfile 表示](onpremisespublishingprofile.md)。

租户管理员可以为每个 **onPremisesPublishingProfile** 配置代理可以 [](updatewindow.md)接收更新或延迟代理更新的时间窗口。 为 **onPremisesPublishingProfile** 指定的更新程序配置适用于该 **onPremisesPublishingProfile 内的所有代理**。 [](hybridagentupdaterconfiguration.md)

有关配置应用程序代理的教程，请参阅使用 [Microsoft Graph API 自动配置应用程序代理](/graph/application-proxy-configure-api)。

## <a name="see-also"></a>另请参阅

- [本地代理](onpremisesagent.md)
- [本地代理组](onpremisesagentgroup.md)
- [本地发布配置文件](onpremisespublishingprofile.md)
- [已发布资源](publishedresource.md)
- [Connector](connector.md)
- [连接器组](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



