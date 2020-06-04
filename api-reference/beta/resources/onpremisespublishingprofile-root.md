---
title: 本地发布配置文件
description: 各种 Azure 服务（例如，Azure Active Directory Connect 直通身份验证、从 Workday 到 Azure AD 用户预配）允许有条件访问公司网络外部的各种本地资源。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3774ceb0a2e03b8c625bf317467c670c93596ac9
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556238"
---
# <a name="on-premises-publishing-profiles"></a>本地发布配置文件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

各种 Azure 服务（例如，Azure Active Directory Connect to [Authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)、 [WORKDAY 到 azure AD 用户预配](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)和[应用程序代理](https://aka.ms/whyappproxy)允许访问公司网络外部的各种本地资源。 可将租户管理员安装的[内部部署代理](onpremisesagent.md)（或应用程序代理的[连接器](connector.md)）配置为将请求路由到特定的[已发布资源](publishedresource.md)。
[代理组](onpremisesagentgroup.md)（或应用程序代理的[连接器组](connectorgroup.md)）使租户管理员能够分配特定代理，以满足特定的已发布内部部署资源。 租户管理员可以将许多代理组合在一起，然后将每个已发布的资源分配给一个组。 同一本地发布类型的整个实体集由[onPremisesPublishingProfile](onpremisespublishingprofile.md)表示。

租户管理员可以为每个**onPremisesPublishingProfile**配置一个[时间](updatewindow.md)段，在此时段内，代理可以接收更新或将更新推迟到代理。 为**onPremisesPublishingProfile**指定的[更新配置](hybridagentupdaterconfiguration.md)适用于该**onPremisesPublishingProfile**中的所有代理。

## <a name="see-also"></a>另请参阅

- [内部部署代理](onpremisesagent.md)
- [内部部署代理组](onpremisesagentgroup.md)
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
