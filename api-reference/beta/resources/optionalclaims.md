---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 6d4bca89a9c1489735eea7e215592395b83f3769
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522135"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="4b137-103">optionalClaims 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b137-103">optionalClaims resource type</span></span>

<span data-ttu-id="4b137-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b137-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b137-105">声明应用程序请求的可选声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="4b137-106">应用程序可以配置可从安全令牌服务接收的三种令牌（ID 令牌、访问令牌、SAML 2 令牌）每种类型中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="4b137-107">应用程序可以配置要在每个令牌类型中返回的一组不同的可选声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="4b137-108">[应用程序](application.md)的 optionalClaims 属性是一个**optionalClaims**对象。</span><span class="sxs-lookup"><span data-stu-id="4b137-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="4b137-109">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="4b137-110">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="4b137-110">See [provide optional claims to your Azure AD app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="4b137-111">属性</span><span class="sxs-lookup"><span data-stu-id="4b137-111">Properties</span></span>
| <span data-ttu-id="4b137-112">属性</span><span class="sxs-lookup"><span data-stu-id="4b137-112">Property</span></span>     | <span data-ttu-id="4b137-113">类型</span><span class="sxs-lookup"><span data-stu-id="4b137-113">Type</span></span>        | <span data-ttu-id="4b137-114">说明</span><span class="sxs-lookup"><span data-stu-id="4b137-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b137-115">idToken</span><span class="sxs-lookup"><span data-stu-id="4b137-115">idToken</span></span>|<span data-ttu-id="4b137-116">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b137-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="4b137-117">JWT ID 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="4b137-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="4b137-118">accessToken</span></span>|<span data-ttu-id="4b137-119">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b137-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="4b137-120">JWT 访问令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="4b137-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="4b137-121">saml2Token</span></span>|<span data-ttu-id="4b137-122">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b137-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="4b137-123">SAML 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="4b137-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b137-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b137-124">JSON Representation</span></span>
<span data-ttu-id="4b137-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b137-125">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}-->
``` json
{
  "idToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "accessToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "saml2Token": [{"@odata.type": "microsoft.graph.optionalClaim"}]
}
```
