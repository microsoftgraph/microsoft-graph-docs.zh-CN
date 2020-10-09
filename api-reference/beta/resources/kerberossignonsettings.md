---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的 kerberos 设置。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 366a220dc8979c55c95706830d4e3d36a920c130
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401145"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="60e4b-103">kerberosSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="60e4b-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="60e4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60e4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e4b-105">表示在通过 Azure AD 应用程序代理发布本地应用程序时， [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) 资源的 Keberos 约束委派 (KCD) 设置。</span><span class="sxs-lookup"><span data-stu-id="60e4b-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="60e4b-106">应用程序代理使用 Kerberos 约束委派 (KCD) 来支持对集成的 Windows 身份验证应用程序的单点登录。</span><span class="sxs-lookup"><span data-stu-id="60e4b-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="60e4b-107">有关详细信息，请参阅 [使用应用程序代理以单点登录到应用的 Kerberos 约束委派](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)。</span><span class="sxs-lookup"><span data-stu-id="60e4b-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="60e4b-108">请勿使用此属性来配置 SAML 或基于密码的单一登录。</span><span class="sxs-lookup"><span data-stu-id="60e4b-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="60e4b-109">如果要配置 SAML 单一登录，则必须在 [servicePrincipal](serviceprincipal.md)上设置此设置。</span><span class="sxs-lookup"><span data-stu-id="60e4b-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="60e4b-110">如果要配置基于密码的单签名，则必须使用 [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)进行设置。</span><span class="sxs-lookup"><span data-stu-id="60e4b-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="60e4b-111">属性</span><span class="sxs-lookup"><span data-stu-id="60e4b-111">Properties</span></span>

| <span data-ttu-id="60e4b-112">属性</span><span class="sxs-lookup"><span data-stu-id="60e4b-112">Property</span></span>     | <span data-ttu-id="60e4b-113">类型</span><span class="sxs-lookup"><span data-stu-id="60e4b-113">Type</span></span>        | <span data-ttu-id="60e4b-114">说明</span><span class="sxs-lookup"><span data-stu-id="60e4b-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60e4b-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="60e4b-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="60e4b-116">字符串</span><span class="sxs-lookup"><span data-stu-id="60e4b-116">String</span></span>| <span data-ttu-id="60e4b-117">应用程序服务器的内部应用程序 SPN。</span><span class="sxs-lookup"><span data-stu-id="60e4b-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="60e4b-118">此 SPN 必须位于连接器可以向其提供委派凭据的服务列表中。</span><span class="sxs-lookup"><span data-stu-id="60e4b-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="60e4b-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="60e4b-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="60e4b-120">字符串</span><span class="sxs-lookup"><span data-stu-id="60e4b-120">String</span></span>| <span data-ttu-id="60e4b-121">代表用户使用的连接器的委派登录标识。</span><span class="sxs-lookup"><span data-stu-id="60e4b-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="60e4b-122">有关详细信息，请参阅使用 [不同的内部部署和云标识 ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)。</span><span class="sxs-lookup"><span data-stu-id="60e4b-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="60e4b-123">可取值为：`userPrincipalName`、`onPremisesUserPrincipalName`、`userPrincipalUsername`、`onPremisesUserPrincipalUsername`、`onPremisesSAMAccountName`。</span><span class="sxs-lookup"><span data-stu-id="60e4b-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60e4b-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60e4b-124">JSON representation</span></span>

<span data-ttu-id="60e4b-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60e4b-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.kerberosSignOnSettings",
  "baseType": null
}-->

```json
{
  "kerberosServicePrincipalName": "String",
  "kerberosSignOnMappingAttributeType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "kerberosSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->