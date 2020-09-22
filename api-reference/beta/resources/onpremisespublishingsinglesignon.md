---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的单一登录设置。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3c2accea8252e8aae9c82bc93ebf92055b13481
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998619"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a><span data-ttu-id="cf88e-103">onPremisesPublishingSingleSignOn 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf88e-103">onPremisesPublishingSingleSignOn resource type</span></span>

<span data-ttu-id="cf88e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf88e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf88e-105">表示在使用 Azure AD 应用程序代理发布本地应用程序时， [onPremisesPublishing](onpremisespublishing.md) 资源的单一登录设置。</span><span class="sxs-lookup"><span data-stu-id="cf88e-105">Represents the single sign-on settings for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Azure AD Application Proxy.</span></span> <span data-ttu-id="cf88e-106">此资源用于将集成的 Windows 身份验证和基于标头的身份验证设置为单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="cf88e-106">This resource is used for setting Integrated Windows Authentication and header-based authentication as the single-sign on mode.</span></span> <span data-ttu-id="cf88e-107">有关详细信息，请参阅 [使用应用程序代理以单点登录到应用的 Kerberos 约束委派](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)。</span><span class="sxs-lookup"><span data-stu-id="cf88e-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="cf88e-108">请勿使用此属性来配置 SAML 或基于密码的单一登录。</span><span class="sxs-lookup"><span data-stu-id="cf88e-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="cf88e-109">如果要配置 SAML 单一登录，则必须在 [servicePrincipal](serviceprincipal.md)上设置此设置。</span><span class="sxs-lookup"><span data-stu-id="cf88e-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="cf88e-110">如果要配置基于密码的单签名，则必须使用 [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)进行设置。</span><span class="sxs-lookup"><span data-stu-id="cf88e-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cf88e-111">属性</span><span class="sxs-lookup"><span data-stu-id="cf88e-111">Properties</span></span>

| <span data-ttu-id="cf88e-112">属性</span><span class="sxs-lookup"><span data-stu-id="cf88e-112">Property</span></span>     | <span data-ttu-id="cf88e-113">类型</span><span class="sxs-lookup"><span data-stu-id="cf88e-113">Type</span></span>        | <span data-ttu-id="cf88e-114">说明</span><span class="sxs-lookup"><span data-stu-id="cf88e-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf88e-115">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="cf88e-115">kerberosSignOnSettings</span></span>| [<span data-ttu-id="cf88e-116">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="cf88e-116">kerberosSignOnSettings</span></span>](kerberossignonsettings.md)| <span data-ttu-id="cf88e-117">使用集成窗口身份验证的应用程序的 Kerberos 约束委派设置。</span><span class="sxs-lookup"><span data-stu-id="cf88e-117">The Kerberos Constrained Delegation settings for applications that use Integrated Window Authentication.</span></span> |
|<span data-ttu-id="cf88e-118">singleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="cf88e-118">singleSignOnMode</span></span>|<span data-ttu-id="cf88e-119">String</span><span class="sxs-lookup"><span data-stu-id="cf88e-119">String</span></span>| <span data-ttu-id="cf88e-120">应用程序的首选单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="cf88e-120">The preferred single-sign on mode for the application.</span></span> <span data-ttu-id="cf88e-121">可取值为：`none`、`onPremisesKerberos`、`headerBased`。</span><span class="sxs-lookup"><span data-stu-id="cf88e-121">Possible values are: `none`, `onPremisesKerberos`, `headerBased`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf88e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf88e-122">JSON representation</span></span>

<span data-ttu-id="cf88e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf88e-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn",
  "baseType": null
}-->

```json
{
  "kerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "singleSignOnMode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingSingleSignOn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

