---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 271fc7a054fce7649ff5b637a0a55d47a566332e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354103"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="fbd57-103">optionalClaims 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbd57-103">optionalClaims resource type</span></span>

<span data-ttu-id="fbd57-104">命名空间： microsoft. graph 声明应用程序请求的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-104">Namespace: microsoft.graph Declares the optional claims requested by an application.</span></span> <span data-ttu-id="fbd57-105">应用程序可以配置可从安全令牌服务接收的三种令牌（ID 令牌、访问令牌、SAML 2 令牌）每种类型中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="fbd57-106">应用程序可以配置要在每个令牌类型中返回的一组不同的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="fbd57-107">[应用程序](application.md)的 optionalClaims 属性是一个**optionalClaims**对象。</span><span class="sxs-lookup"><span data-stu-id="fbd57-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="fbd57-108">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="fbd57-109">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="fbd57-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="fbd57-110">属性</span><span class="sxs-lookup"><span data-stu-id="fbd57-110">Properties</span></span>
| <span data-ttu-id="fbd57-111">属性</span><span class="sxs-lookup"><span data-stu-id="fbd57-111">Property</span></span>     | <span data-ttu-id="fbd57-112">类型</span><span class="sxs-lookup"><span data-stu-id="fbd57-112">Type</span></span>        | <span data-ttu-id="fbd57-113">说明</span><span class="sxs-lookup"><span data-stu-id="fbd57-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fbd57-114">idToken</span><span class="sxs-lookup"><span data-stu-id="fbd57-114">idToken</span></span>|<span data-ttu-id="fbd57-115">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbd57-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="fbd57-116">JWT ID 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="fbd57-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="fbd57-117">accessToken</span></span>|<span data-ttu-id="fbd57-118">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbd57-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="fbd57-119">JWT 访问令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="fbd57-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="fbd57-120">saml2Token</span></span>|<span data-ttu-id="fbd57-121">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbd57-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="fbd57-122">SAML 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fbd57-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbd57-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbd57-123">JSON Representation</span></span>
<span data-ttu-id="fbd57-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbd57-124">Here is a JSON representation of the resource.</span></span>
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