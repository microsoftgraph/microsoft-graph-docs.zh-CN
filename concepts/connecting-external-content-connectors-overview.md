---
title: Microsoft Graph 连接器概述
description: Microsoft Graph 连接器概述
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: a14435329e99dba4c9ec6710c36f91a05655d0e711deab3994e58d18e853253b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54151815"
---
# <a name="microsoft-graph-connectors-overview"></a>Microsoft Graph 连接器概述

[Microsoft 365](https://www.microsoft.com/microsoft-365) 是一套完整的智能解决方案，可让用户和组织获得创新生产力体验和丰富见解，从而提高效率、促进业务增长。 Microsoft Graph 是支持这些智能体验的数据平台，Microsoft Graph API 提供此数据和智能的访问权限。

尽管大多数信息工作者在生产力应用程序（如 [Microsoft 365](https://www.microsoft.com/microsoft-365)）上花费大量时间，但他们也需要一种方法将环境与企业应用程序以及他们使用的其他本地和 SaaS 云软件和服务集成。 例如，企业资源计划 （ERP） 应用程序、客户资源管理 （CRM） 应用程序、Intranet 应用程序、Wiki、博客和社交网络网站。

Microsoft Graph 连接器提供了一种简单直观的方法，可将外部服务中的内容引入 Microsoft Graph，为 Microsoft 365 智能体验提供支持，如 Microsoft Search（当前 GA）以及即将推出许多如 Viva 主题等。

现在，使用 Microsoft Graph 连接器，你引入组织的数据可能出现在 Microsoft 搜索结果中。 此功能扩展了 Microsoft 365 生产力应用中可搜索的内容源类型以及 Microsoft 更广泛的数据源。 不久将，连接器将支持许多其他 Microsoft 365 智能体验。
下图提供了 Microsoft Graph 连接线高级概述。

<!---Insert image reference here --->
<!---       ![Select the Microsoft Graph permissions](./images/application-saml-sso-configure-api/set-permissions.png) --->
![图像显示正使用连接线将数据引入 Microsoft Graph](./images/connectors-images/overview.png)

## <a name="build-your-own-custom-connector"></a>构建自己的自定义连接器

Microsoft 和合作伙伴当前提供的 100 多个连接器可用于连接到热门的 Microsoft 和非 Microsoft 服务。 现有连接器的示例包括 Azure 服务、Box、ServiceNow、SalesForce、Google 服务、MediaWiki 等。

若要详细了解现有的 Microsoft Graph 连接器，请访问 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)。

尽管这些连接器有助于连接到流行的服务，但您可能希望与现有[连接器库](/microsoftsearch/connectors-gallery)中未提供的服务进行集成。 您可以使用 Microsoft Graph connectors API 构建自定义连接器，将外部数据引入 Microsoft 365 体验，包括 Microsoft Search、Viva 主题等（即将推出）。

## <a name="get-started-with-custom-graph-connectors"></a>自定义图形连接线入门：
* [使用连接器 API](connecting-external-content-connectors-api-overview.md)
* [将 Postman 与 Microsoft Graph 连接器 API 一并使用](connecting-external-content-connectors-api-postman.md)
<!---**(Articles coming next)**
* [Build your first custom connector with Microsoft Graph]()
--->

