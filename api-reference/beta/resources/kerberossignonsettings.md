---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的 kerberos 设置。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: af00e70e1ef4603c1b1370ec5ef9e9ba75fecb4c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943658"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="f0963-103">kerberosSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0963-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="f0963-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0963-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0963-105">通过 Azure AD 应用程序代理发布本地应用程序时，代表 [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) 资源的 Keberos 约束委派 (KCD) 设置。</span><span class="sxs-lookup"><span data-stu-id="f0963-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="f0963-106">应用程序代理使用 Kerberos 约束 (KCD) 支持对集成 Windows 身份验证应用程序进行单一登录。</span><span class="sxs-lookup"><span data-stu-id="f0963-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="f0963-107">有关详细信息，请参阅 [Kerberos 约束委派，以使用应用程序代理单一登录应用](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)。</span><span class="sxs-lookup"><span data-stu-id="f0963-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="f0963-108">请勿使用此属性配置 SAML 或基于密码的单一登录。</span><span class="sxs-lookup"><span data-stu-id="f0963-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="f0963-109">如果要配置 SAML 单一登录，则必须在[servicePrincipal 上设置。](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="f0963-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="f0963-110">如果要配置基于密码的单一签名，必须使用 [createPasswordSingleSignOnCredentials 进行设置](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)。</span><span class="sxs-lookup"><span data-stu-id="f0963-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0963-111">属性</span><span class="sxs-lookup"><span data-stu-id="f0963-111">Properties</span></span>

| <span data-ttu-id="f0963-112">属性</span><span class="sxs-lookup"><span data-stu-id="f0963-112">Property</span></span>     | <span data-ttu-id="f0963-113">类型</span><span class="sxs-lookup"><span data-stu-id="f0963-113">Type</span></span>        | <span data-ttu-id="f0963-114">说明</span><span class="sxs-lookup"><span data-stu-id="f0963-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0963-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0963-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="f0963-116">String</span><span class="sxs-lookup"><span data-stu-id="f0963-116">String</span></span>| <span data-ttu-id="f0963-117">应用程序服务器的内部应用程序 SPN。</span><span class="sxs-lookup"><span data-stu-id="f0963-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="f0963-118">此 SPN 需在连接器可以呈现委派凭据的服务列表中。</span><span class="sxs-lookup"><span data-stu-id="f0963-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="f0963-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="f0963-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="f0963-120">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="f0963-120">kerberosSignOnMappingAttributeType</span></span>| <span data-ttu-id="f0963-121">代表用户使用的连接器的委派登录标识。</span><span class="sxs-lookup"><span data-stu-id="f0963-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="f0963-122">有关详细信息，请参阅使用不同的本地 [和云标识 ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)。</span><span class="sxs-lookup"><span data-stu-id="f0963-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="f0963-123">可取值为：`userPrincipalName`、`onPremisesUserPrincipalName`、`userPrincipalUsername`、`onPremisesUserPrincipalUsername`、`onPremisesSAMAccountName`。</span><span class="sxs-lookup"><span data-stu-id="f0963-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0963-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0963-124">JSON representation</span></span>

<span data-ttu-id="f0963-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0963-125">The following is a JSON representation of the resource.</span></span>

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
