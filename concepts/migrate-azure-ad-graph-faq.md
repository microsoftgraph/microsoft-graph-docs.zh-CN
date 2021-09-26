---
title: Azure Active Directory (Azure AD) Graph Microsoft Graph迁移常见问题解答
description: Azure Active Directory (Azure AD) Graph Microsoft Graph迁移常见问题解答。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 93d5fe0df29b09b083c15a2287b4f47dc6fe166f
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763350"
---
# <a name="azure-active-directory-azure-ad-graph-to-microsoft-graph-migration-faq"></a>Azure Active Directory (Azure AD) Graph Microsoft Graph迁移常见问题解答

本文提供了有关从 Azure AD 服务器迁移到 Microsoft Graph的常见问题Graph。

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Microsoft Graph Azure AD Graph，为什么应该迁移我的应用？

Azure AD Graph API 仅提供对 Azure AD 服务的访问权限。 Microsoft Graph API 提供了一个统一终结点，用于访问 Azure AD 服务和其他 Microsoft 服务 如 Microsoft Teams、Microsoft Exchange 和 Microsoft Intune。

Microsoft Graph还比 Azure AD Graph。 因此，Azure AD Graph自 2020 年 6 月 30 日开始弃用，将于 2022 年 6 月 30 日停用。 2022 年 6 月 30 日之后，应用将不再收到来自 Azure AD Graph响应。 迁移到 Microsoft Graph以避免功能丢失。

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>作为开发人员，如何识别使用 Azure AD Graph？

按照以下步骤识别依赖 Azure AD 应用Graph：

### <a name="step-1-scan-the-application-source-code"></a>步骤 1：扫描应用程序源代码

如果您拥有应用程序的源代码，则搜索 `https://graph.windows.net/` 代码中的 URI。 这是 Azure AD Graph终结点，调用此终结点的应用使用 Azure AD Graph。 记录受影响应用的应用 ID 的值。

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>步骤 2：在 Azure 门户上检查应用的 API 权限

1. 以全局 [管理员角色](https://portal.azure.com) 登录到 Azure 门户。
1. 搜索并选择 **"Azure Active Directory"。**
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在应用 **注册窗口中** ，启用 **应用注册搜索预览**。 选择" **所有应用程序"** 选项卡，然后选择" **添加筛选器"** 选项。 从可用 **筛选器 (选择**) 客户端客户端 ID"选项，然后选择"应用 **"。**  将弹出筛选器。
1. 在文本框中，输入你在步骤 1 中检索到的应用 ID， **然后选择应用**。 该列表已缩小到指定的应用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="按应用 ID 按应用进行筛选。" border="true":::

1. 选择应用。 这将显示应用的菜单。
1. 从窗口的左侧窗格中，选择 **"API 权限"。** 这将显示为应用配置的 API 权限，包括 Azure AD Graph权限。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/configuredPermissions.png" alt-text="Azure 门户中的应用的 API 权限列表。" border="true":::


## <a name="as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph"></a>作为 IT 管理员，如何在租户中标识使用 Azure AD Graph？

使用以下三种方法之一在租户中标识依赖 Azure AD Graph。

### <a name="method-1-through-network-proxy-logs"></a>方法 1：通过网络代理日志

针对调用终结点的任何应用，通过筛选器代理检查网络服务器流量 `https://graph.windows.net/` 日志。 这些应用使用 Azure AD Graph。

### <a name="method-2-use-the-app-registrations-menu-of-the-azure-portal"></a>方法 2：使用 Azure 门户的应用注册菜单

1. 以全局 [管理员角色](https://portal.azure.com) 登录到 Azure 门户。
1. 搜索并选择 **"Azure Active Directory"。**
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在应用 **注册窗口中** ，启用 **应用注册搜索预览**。 选择" **所有应用程序"** 选项卡，然后选择" **添加筛选器"** 选项。 从可用 **筛选器列表中选择"请求的 API"** 选项，然后选择"应用 **"。** 将 **弹出请求的 API** 筛选器。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="按应用请求的 API 筛选应用。" border="true":::

5. 选择 **"Microsoft API"。** 选择 **Please select an API** drop down and choose **Azure Active Directory Graph**. 选择“**应用**”。 这将列出在 Azure AD 应用程序上具有依赖项的所有Graph。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="筛选使用 Azure AD Graph。" border="true":::

### <a name="method-3-use-a-powershell-script"></a>方法 3：使用 PowerShell 脚本

下载并运行 [此 PowerShell 脚本](https://github.com/microsoft/AzureADGraphApps)。



## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>Microsoft 向我发送了一封电子邮件，其中列出了使用 Azure AD Graph 的应用的应用GRAPH。 如何查找每个应用的详细信息，包括其所有者？

1. 以全局 [管理员角色](https://portal.azure.com) 登录到 Azure 门户。
1. 搜索并选择 **"Azure Active Directory"。**
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在应用 **注册窗口中** ，启用 **应用注册搜索预览**。 选择" **所有应用程序"** 选项卡，然后选择" **添加筛选器"** 选项。 从可用 **筛选器 (选择**) 客户端客户端 ID"选项，然后选择"应用 **"。**  将弹出筛选器。
1. 在文本框中输入应用 ID， **然后选择应用**。 该列表已缩小到指定的应用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="按应用 ID 按应用进行筛选。" border="true":::

6. 选择应用。 这将显示应用的菜单。 从窗口的左窗格中，菜单选项（如 **所有者** ）允许你检索应用的详细信息。

## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-are-these-all-the-affected-apps"></a>Microsoft 向我发送了一封电子邮件，其中列出了使用 Azure AD Graph 的应用的应用GRAPH。 这是否所有受影响的应用？

此列表仅捕获过去 28 天内使用的应用和调用 Azure AD Graph终结点。 由于某些应用可能有季节性使用，因此其应用 ID 可能会捕获到一个月的列表中，而不是在另一个列表中。 若要检索受影响应用的完整列表，我们建议你遵循前面列出的 [三种方法](#as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph) 之一。

## <a name="im-a-subscription-owner-and-microsoft-sent-me-an-email-about-azure-ad-graph-deprecation-with-a-list-of-app-ids-what-should-i-do"></a>我是订阅所有者，Microsoft 向我发送了一封有关 Azure AD Graph弃用的应用 ID 列表的电子邮件。 我该怎么办？

你收到的电子邮件包括链接到应用 ID 的租户 ID。 按照以下步骤检索特定租户的技术联系人详细信息。
1. 以管理员角色 [登录到 Azure](https://portal.azure.com) 门户。
1. 如果你是多个 Azure AD 租户中的订阅所有者，请首先切换到相关租户或目录。
    1. 在窗口的右上角，选择你的配置文件图标，然后选择 **切换目录**。 这将显示 **门户|目录 + 订阅** 窗口。 
    1. 从列表中，使用"切换"选项卡切换到其目录 ID 与你在电子邮件中收到的租户 ID 匹配的目录。 Active Directory 标记为"当前 **"。**
    1. 关闭该窗口。
1. 在相关目录中，搜索并选择 **"Azure Active Directory"。** 这将显示活动租户的菜单。 
1. 从窗口左侧窗格的"管理"下 **，** 选择"属性 **"。**
1. 在 **"租户属性** "窗口中，首先验证租户 ID 的值是否与你在电子邮件中收到的租户 ID 匹配。 检索 **技术联系人** 详细信息以与租户联系，以便他们了解弃用。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/tenantTechnicalContact.png" alt-text="查找租户的技术联系人。" border="true":::

## <a name="i-know-apps-that-are-using-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph"></a>我了解使用 Azure AD Graph。 如何将它们迁移到 Microsoft Graph？

若要将应用从 Azure AD Graph Microsoft Graph，请按照[应用迁移规划清单操作](migrate-azure-ad-graph-planning-checklist.md)。

## <a name="i-dont-own-some-apps-in-my-tenant-but-they-use-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph-api-can-i-find-the-owner-of-such-apps"></a>我在我的租户中不拥有某些应用，但它们使用 Azure AD Graph。 如何将它们迁移到 Microsoft Graph API？ 我能否找到此类应用的所有者？

首先，确认租户拥有的应用的完整列表或集成在租户中的第三方应用程序的完整列表。

1. 以管理员角色 [登录到 Azure](https://portal.azure.com) 门户。
1. 搜索并选择 **"Azure Active Directory"。**
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在"应用注册"窗口中，选择" **所有应用程序"** 选项卡。
1. 选择应用。 这将显示应用的菜单。
1. 在窗口的左窗格中，菜单选项显示应用的详细信息（包括其所有者）。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppOwners.png" alt-text="查找应用所有者。" border="true":::


## <a name="can-i-request-for-an-exception-if-im-unable-to-meet-the-june-30-2022-migration-deadline"></a>如果我无法满足 2022 年 6 月 30 日迁移截止时间的要求，我能否请求例外？  

此弃用没有例外情况。 2022 年 6 月 30 日之后，应用将不再Graph Azure AD 终结点收到响应。 

## <a name="i-need-to-create-new-apps-to-use-azure-ad-graph-but-the-azure-ad-graph-api-permission-sign-up-is-closed-how-can-i-create-my-app"></a>我需要创建新应用以使用 Azure AD Graph但 Azure AD Graph API 权限注册已关闭。 如何创建我的应用程序？

首先，我们建议你遵循应用迁移[规划清单](migrate-azure-ad-graph-planning-checklist.md)来帮助你将应用转换为 Microsoft Graph API。 

如果你发现了 Microsoft Graph不支持 Azure AD Graph 支持的功能的空白，请与租户管理员或订阅所有者一起报告此缺陷。 当我们确认这确实存在 Microsoft Graph API 未达到的空白时，我们将帮助你创建应用。 但是，这并不意味着弃用是例外。 使用 Azure AD Graph应用在 2022 年 6 月 30 日之后仍将停止运行。


## <a name="see-also"></a>另请参阅

+ [应用迁移清单](migrate-azure-ad-graph-request-differences.md)
