---
title: 从云解决方案提供商应用程序中调用 Microsoft Graph
description: 本主题介绍如何使应用程序使用授权代码授予流或服务到服务客户端凭据流，通过 Microsoft Graph 访问合作伙伴托管的客户数据。
author: jackson-woods
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 8c610b1d795045c49b469ceb906a9994a4020b3a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021391"
---
# <a name="call-microsoft-graph-from-a-cloud-solution-provider-application"></a>从云解决方案提供商应用程序中调用 Microsoft Graph

> **注意：** 本主题 **仅** 适用于 Microsoft 云解决方案提供商 (CSP) 应用程序开发者。[Microsoft 云解决方案提供商 (CSP)](https://partner.microsoft.com/cloud-solution-provider) 计划使 Microsoft 的合作伙伴可以管理 Microsoft Online Services 并将其转售给客户。

本主题介绍如何使应用程序使用[授权代码授予流](/azure/active-directory/develop/active-directory-protocols-oauth-code)或[服务到服务客户端凭据流](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)，通过 Microsoft Graph 访问合作伙伴托管的客户数据。

**重要说明：** 从 CSP 应用程序中调用 Microsoft Graph 仅受目录资源（例如 **用户**、**组**、**设备**、**组织**）和 [Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-beta) 资源支持。

## <a name="what-is-a-partner-managed-application"></a>什么是合作伙伴托管的应用程序

CSP 计划使 Microsoft 的合作伙伴可以管理 Microsoft Online Services（例如 Microsoft 365、Microsoft Azure 和 CRM Online）并将其转售给客户。客户服务的管理是通过委派管理员特权完成的，这使委派的合作伙伴用户（称为代理）可以访问并配置其客户的环境。

此外，作为合作伙伴开发者，你可以构建 **合作伙伴托管的应用** 来管理客户的 Microsoft 服务。合作伙伴托管的应用通常称为 *预先同意的* 应用，因为所有客户都已自动预先同意合作伙伴托管的应用。这意味着，当某个客户租户中的用户使用一个合作伙伴托管的应用时，用户不会收到给予同意的提示就能使用该应用。合作伙伴托管的应用还可以继承委派的管理员特权，因此，你的合作伙伴代理还可以通过合作伙伴托管的应用程序获取对客户的特权访问。

## <a name="how-to-set-up-a-partner-managed-application"></a>如何设置合作伙伴托管的应用程序

被授予访问客户数据的提升权限时，应用程序被视为 *合作伙伴托管*。

> **注意：** 合作伙伴托管的应用 *仅* 可以在合作伙伴租户中配置，为管理客户租户资源，合作伙伴托管的应用 **必须** 配置为 **多租户应用程序**。

### <a name="register-and-configure-a-multi-tenant-app"></a>注册和配置多租户应用

此处所需的初始步骤与注册和配置多租户应用程序所用的步骤相同：

1. 使用 [Azure 门户](https://portal.azure.com)在合作伙伴租户中[注册应用程序](/azure/active-directory/active-directory-app-registration)。若要作为合作伙伴托管的应用，必须将应用程序配置为[多租户应用](/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant)。此外，如果应用已经过部署并在多个地理区域中销售，你将需要如<a href="#region">此处</a>所述在每个区域中注册你的应用。
2. 使用最低特权的方法，再次通过 Azure 门户为多租户应用配置需要的 *必要权限*。

### <a name="pre-consent-your-app-for-all-your-customers"></a>为你的所有客户预先同意应用

为你的所有客户最终授予合作伙伴托管的应用的已配置权限。你可以通过使用 Azure AD powershell V2 将代表应用的 **servicePrincipal** 添加到合作伙伴租户中的 *Adminagents* 组，以执行此操作。你可以在 [此处](https://www.powershellgallery.com/packages/AzureAD)下载和安装 Azure AD PowerShell V2。按照以下步骤查找 *Adminagents* 组、**servicePrincipal** 并将其添加到组。

1. 打开 PowerShell 会话，并通过在登录窗口中输入管理员凭据连接到合作伙伴租户。

    ```PowerShell
    Connect-AzureAd
    ```

2. 查找代表 *Adminagents* 的组。

    ```PowerShell
    $group = Get-AzureADGroup -Filter "displayName eq 'Adminagents'"
    ```

3. 查找与应用具有相同 *appId* 的服务主体。

    ```PowerShell
    $sp = Get-AzureADServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. 最后，将服务主体添加到 *Adminagents* 组中。

    ```PowerShell
    Add-AzureADGroupMember -ObjectId $group.ObjectId -RefObjectId $sp.ObjectId
    ```

## <a name="token-acquisition-flows"></a>令牌购置流

合作伙伴托管的应用的令牌购置流（[授权代码授予流](/azure/active-directory/develop/active-directory-protocols-oauth-code)和[服务到服务客户端凭据流](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)）与常规的多租户应用相同。

除了预先同意访问所有客户租户外，合作伙伴托管的应用还具有其他功能。它允许你的代理使用应用访问客户的租户数据（使用委派的管理员特权）。从概念上讲，工作原理如下：

1. 代理使用从合作伙伴租户颁发的用户凭据登录你的应用。
2. 你的应用请求对目标合作伙伴托管的客户租户的访问令牌。
3. 你的应用使用访问令牌调用 Microsoft Graph。

除了代理必须使用其合作伙伴帐户登录之外，这是标准的 [授权代码授予流](/azure/active-directory/develop/active-directory-protocols-oauth-code)。若要查看其工作原理，请假设你的合作伙伴租户是 *partner.com*（这是代理的主租户），并将你的一位客户假设为 *customer.com*：

1. [获取授权代码：](/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code)在我们的示例 ```customer.com``` 中，对于目标租户，你的应用会对 ```/authorize``` 终结点发出请求，且必须使用 **客户租户** 你的代理将仍然使用其 ```username@partner.com``` 帐户登录。

    ```http
    GET https://login.microsoftonline.com/customer.com/oauth2/authorize
    ```

2. [使用授权代码获取访问令牌：](/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token)在我们的示例 ```customer.com``` 中，当对 ```token``` 终结点发出请求时，你的应用必须将 **客户租户** 用作目标租户：

    ```http
    POST https://login.microsoftonline.com/customer.com/oauth2/token
    ```

3. 现在你拥有了访问令牌，请调用 Microsoft Graph，将访问令牌置于 HTTP 授权标头中：

    ```http
    GET https://graph.microsoft.com/beta/users
    Authorization: Bearer <token>
    ```

## <a name="register-your-app-in-the-regions-you-support"></a>在支持的区域中注册你的应用
<a name="region"></a>

CSP 客户服务当前仅限于单个区域。合作伙伴托管的应用程序执行相同的限制。这意味着你在进行销售的每个区域必须具有单独的租户。例如，如果合作伙伴托管的应用在位于美国的租户中注册，但你的客户位于英国，合作伙伴托管的应用将无法工作。每个区域合作伙伴租户必须维护自己的一组合作伙伴托管的应用，才能管理相同区域内的客户。这可能需要应用中的其他逻辑（登录前）获取用户的登录用户名，才能决定使用哪个特定于区域的合作伙伴托管的标识来为用户提供服务。

## <a name="calling-microsoft-graph-immediately-after-customer-creation"></a>创建客户后立即调用 Microsoft Graph

使用[合作伙伴中心 API](https://partnercenter.microsoft.com/partner/developer) 创建新客户时会创建新的客户租户。此外，还会创建合作伙伴关系，这使你成为此新客户租户的在案合作伙伴。这种伙伴关系可能需要最多 3 分钟传播给新客户租户。如果应用在创建后直接调用 Microsoft Graph，应用可能会接收拒绝访问错误。当现有客户接受你的邀请时可能会遇到类似延迟。这是因为预先同意依赖于客户租户中现已存在的合作伙伴关系。

为避免此问题，在调用 Azure AD 以获取令牌（从而调用 Microsoft Graph）之前，我们建议你的合作伙伴应用应在创建客户后等待 **三分钟**。 这应该涵盖了大多数情况。 但是，如果等待三分钟后仍收到授权错误，请再等待 60 秒后重试。

> **注意：** 重试时，你必须在调用 Microsoft Graph 之前从 Azure AD 获取新的访问令牌。你将无法使用已经拥有的访问令牌调用 Microsoft Graph，因为访问令牌只能使用一小时，且不包含预先同意的权限声明。
