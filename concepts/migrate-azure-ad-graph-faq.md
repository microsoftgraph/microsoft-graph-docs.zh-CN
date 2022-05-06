---
title: Azure AD Graph到 Microsoft Graph 迁移常见问题解答
description: 提供有关从Azure Active Directory (Azure AD) Graph迁移到 Microsoft Graph 的常见问题的解答。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 0605dfc2eb38f6339fe27f167599a211d1c80208
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247068"
---
# <a name="azure-ad-graph-to-microsoft-graph-migration-faq"></a>Azure AD Graph到 Microsoft Graph 迁移常见问题解答

本文提供有关从Azure Active Directory (Azure AD) Graph迁移到 [Microsoft Graph](/graph/overview) 的常见问题的解答。

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Microsoft Graph与Azure AD Graph有何不同，为何要迁移应用？

Azure AD 图形 API仅提供对Azure AD服务的访问权限。 Microsoft 图形 API提供单个统一终结点，用于访问Azure AD服务和其他Microsoft 服务，例如Microsoft Teams、Microsoft Exchange和Microsoft Intune。

[与Azure AD Graph相比，Microsoft Graph](/graph/overview)的安全性和复原能力也更高。 因此，Azure AD Graph自 2020 年 6 月 30 日起一直处于弃用状态，在将所有投资转移到 Microsoft Graph 时，将于近期停用。 停用后，应用将从Azure AD Graph终结点收到错误响应。 迁移到 Microsoft Graph以避免功能丢失。

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>作为开发人员，如何识别使用Azure AD Graph的应用？

按照以下步骤识别依赖于Azure AD Graph的应用：

### <a name="step-1-scan-the-application-source-code"></a>步骤 1：扫描应用程序源代码

如果拥有应用程序的源代码，请在代码中搜索 `https://graph.windows.net/` URI。 这是调用此终结点的Azure AD Graph终结点和应用使用Azure AD Graph。 记录受影响应用的应用 ID 的值。

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>步骤 2：检查应用对Azure 门户的 API 权限

1. 以全局管理员身份登录[到Azure 门户](https://portal.azure.com)。
1. 搜索并选择 **Azure Active Directory**。
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在 **应用注册** 窗口中，启用 **应用注册搜索预览**。 选择“ **所有应用程序** ”选项卡，然后选择 **“添加筛选器** ”选项。 从可用筛选器列表中选择应用程序 **(客户端) ID** 选项，然后选择 **“应用**”。  弹出一个筛选器。
1. 在文本框中，输入在步骤 1 中检索到的应用 ID，然后选择 **“应用**”。 列表已缩小到指定的应用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="按应用 ID 按应用筛选。" border="true":::

1. 选择应用。 这会显示应用的菜单。
1. 在窗口的左窗格中，选择 **API 权限**。 这会显示为应用配置的 API 权限，包括Azure AD Graph权限。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/configuredPermissions.png" alt-text="来自Azure 门户的应用的 API 权限列表。" border="true":::


## <a name="as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph"></a>作为 IT 管理员，如何识别租户中使用Azure AD Graph的应用？

使用以下三种方法之一来标识租户中依赖于Azure AD Graph的应用。

### <a name="method-1-through-network-proxy-logs"></a>方法 1：通过网络代理日志

通过筛选器代理检查调用终结点的任何应用的 `https://graph.windows.net/` 网络服务器流量日志。 这些应用使用Azure AD Graph。

### <a name="method-2-use-the-app-registrations-menu-of-the-azure-portal"></a>方法 2：使用Azure 门户的应用注册菜单

1. 以全局管理员身份登录[到Azure 门户](https://portal.azure.com)。
1. 搜索并选择 **Azure Active Directory**。
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在 **应用注册** 窗口中，启用 **应用注册搜索预览**。 选择“ **所有应用程序** ”选项卡，然后选择 **“添加筛选器** ”选项。 从可用筛选器列表中选择 **“请求的 API** ”选项，然后选择 **“应用**”。 “ **请求的 API** 筛选器”弹出。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="按所请求的 API 筛选应用。" border="true":::

5. 选择 **Microsoft API**。 选择 **“请选择 API**”下拉列表，然后选择 **Azure Active Directory Graph**。 选择“**应用**”。 这会列出依赖于Azure AD Graph的所有应用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="筛选使用Azure AD Graph的应用。" border="true":::

### <a name="method-3-use-a-powershell-script"></a>方法 3：使用 PowerShell 脚本

下载并运行 [此 PowerShell 脚本](https://github.com/microsoft/AzureADGraphApps)。 使用此方法可在租户中检索具有其主目录的应用，并在其他租户中使用其主目录检索应用。


## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>Microsoft 向我发送了一封电子邮件，其中包含使用Azure AD Graph的应用的应用 ID 列表。 如何实现找到每个应用的详细信息，包括其所有者？

1. 以全局管理员身份登录[到Azure 门户](https://portal.azure.com)。
1. 搜索并选择 **Azure Active Directory**。
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在 **应用注册** 窗口中，启用 **应用注册搜索预览**。 选择“ **所有应用程序** ”选项卡，然后选择 **“添加筛选器** ”选项。 从可用筛选器列表中选择应用程序 **(客户端) ID** 选项，然后选择 **“应用**”。  弹出一个筛选器。
1. 在文本框中输入应用 ID，然后选择 **“应用**”。 列表已缩小到指定的应用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="按应用 ID 按应用筛选。" border="true":::

6. 选择应用。 这会显示应用的菜单。 在窗口的左窗格中， **使用“所有者”** 等菜单选项可以检索应用的详细信息。

## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-are-these-all-the-affected-apps"></a>Microsoft 向我发送了一封电子邮件，其中包含使用Azure AD Graph的应用的应用 ID 列表。 这些是所有受影响的应用吗？

此列表仅捕获过去 28 天内使用的应用，并调用Azure AD Graph终结点。 由于某些应用可能具有季节性使用，因此它们的应用 ID 可能会在一个月的列表中捕获，但不会在另一个月中捕获。 若要检索受影响应用的完整列表，建议遵循前面列出的 [三种方法](#as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph) 之一。

## <a name="im-a-subscription-owner-and-microsoft-sent-me-an-email-about-azure-ad-graph-deprecation-with-a-list-of-app-ids-what-should-i-do"></a>我是订阅所有者，Microsoft 向我发送了一封关于使用应用 ID 列表Azure AD Graph弃用的电子邮件。 我该怎么办？

收到的电子邮件包括链接到应用 ID 的租户 ID。 按照以下步骤检索特定租户的技术联系人详细信息。
1. 以管理员身份登录到[Azure 门户](https://portal.azure.com)。
1. 如果你是多个Azure AD租户中的订阅所有者，请先切换到相关的租户或目录。
    1. 在窗口右上角，选择配置文件图标，然后选择 **“切换目录**”。 这会显示 **门户设置|“目录 + 订阅”** 窗口。 
    1. 在列表中，使用 **“切换”** 选项卡切换到目录 ID 与电子邮件中收到的租户 ID 匹配的目录。 活动目录标记为 **“当前**”。
    1. 关闭该窗口。
1. 在相关目录中，搜索并选择 **Azure Active Directory**。 这会显示活动租户的菜单。 
1. 在窗口左窗格的“ **管理”** 下，选择 **“属性**”。
1. 在 **“租户属性** ”窗口中，首先验证租户 ID 的值是否与电子邮件中收到的租户 ID 相匹配。 检索 **技术联系人** 详细信息以联系租户，以便他们能够知道弃用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/tenantTechnicalContact.png" alt-text="查找租户的技术联系人。" border="true":::

## <a name="i-know-apps-that-are-using-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph"></a>我知道正在使用Azure AD Graph的应用。 如何实现将其迁移到 Microsoft Graph？

若要将应用从Azure AD Graph迁移到 Microsoft Graph，请按照[应用迁移计划清单](migrate-azure-ad-graph-planning-checklist.md)进行操作。

## <a name="i-dont-own-some-apps-in-my-tenant-but-they-use-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph-api-can-i-find-the-owner-of-such-apps"></a>我的租户中没有一些应用，但它们使用Azure AD Graph。 如何实现将其迁移到 Microsoft 图形 API？ 能否找到此类应用的所有者？

首先，确认租户或第三方应用程序在租户中集成的应用的完整列表。

1. 以管理员身份登录到[Azure 门户](https://portal.azure.com)。
1. 搜索并选择 **Azure Active Directory**。
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在应用注册窗口中，选择“**所有应用程序**”选项卡。
1. 选择应用。 这会显示应用的菜单。
1. 在窗口的左窗格中，菜单选项显示应用的详细信息，包括其所有者。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppOwners.png" alt-text="查找应用所有者。" border="true":::


## <a name="my-organization-runs-azure-stack-hub-what-actions-should-i-take"></a>我的组织运行 Azure Stack Hub。 我应该采取什么措施？

如果组织运行 Azure Stack Hub，则最重要的操作是遵循 [Azure Stack Hub 服务策略](/azure-stack/operator/azure-stack-servicing-policy)。

若要迁移，将通过 Azure Stack Hub 管理门户通知客户更新其主租户和来宾租户目录。 迁移到 Microsoft Graph 将由集成系统更新体验进行管理。

## <a name="i-need-to-add-new-azure-ad-graph-permissions-to-my-app-but-i-cant-select-azure-ad-graph-as-a-required-permission-for-my-app-registration-how-can-i-add-the-azure-ad-graph-permissions"></a>我需要向应用添加新的Azure AD Graph权限，但无法选择Azure AD Graph作为应用注册所需的权限。 如何添加Azure AD Graph权限？

首先，建议遵循[应用迁移规划清单](migrate-azure-ad-graph-planning-checklist.md)，帮助你将应用转换为 Microsoft 图形 API。

如果发现 Microsoft Graph不支持Azure AD Graph中提供的功能的差距，请使用标记 [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html) 通过 Microsoft Q&A 告知我们。

如果仍需要为应用程序配置Azure AD Graph权限，请使用以下解决方法之一。

+ 使用Azure 门户查找组织使用的 API
+ 更新Azure 门户上的应用程序清单
+ 使用 Microsoft Graph中的[应用程序](/graph/api/resources/application) API 更新 [requiredResourceAccess](/graph/api/resources/requiredresourceaccess) 对象
+ 在 Microsoft Graph PowerShell SDK 中使用 [Update-MgApplicationcmdlet](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) 

有关使用列出的解决方法的示例，请参阅[使用 Microsoft Graph 配置应用注册所需的Azure AD Graph](migrate-azure-ad-graph-configure-permissions.md)权限

>**注意：** 停用Azure AD Graph后，不支持使用这些解决方法添加Azure AD Graph权限。 停用后，使用Azure AD Graph的任何应用仍将停止运行。



## <a name="see-also"></a>另请参阅

+ [应用迁移清单](migrate-azure-ad-graph-request-differences.md)
