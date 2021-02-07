---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 2830aef91557346d3d02249d35df41eccffa565e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136218"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="fb749-103">optionalClaims 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb749-103">optionalClaims resource type</span></span>

<span data-ttu-id="fb749-104">命名空间：microsoft.graph 声明应用程序请求的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fb749-104">Namespace: microsoft.graph Declares the optional claims requested by an application.</span></span> <span data-ttu-id="fb749-105">应用程序可以配置可选声明，以在三种类型的令牌中返回 (ID 令牌、访问令牌、SAML 2 令牌) 它可以从安全令牌服务接收。</span><span class="sxs-lookup"><span data-stu-id="fb749-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="fb749-106">应用程序可以配置一组不同的可选声明，以在每个令牌类型中返回。</span><span class="sxs-lookup"><span data-stu-id="fb749-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="fb749-107">应用程序的 optionalClaims 属性 [是](application.md)**可选Claims** 对象。</span><span class="sxs-lookup"><span data-stu-id="fb749-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="fb749-108">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="fb749-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="fb749-109">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="fb749-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="fb749-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb749-110">Properties</span></span>
| <span data-ttu-id="fb749-111">属性</span><span class="sxs-lookup"><span data-stu-id="fb749-111">Property</span></span>     | <span data-ttu-id="fb749-112">类型</span><span class="sxs-lookup"><span data-stu-id="fb749-112">Type</span></span>        | <span data-ttu-id="fb749-113">说明</span><span class="sxs-lookup"><span data-stu-id="fb749-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb749-114">idToken</span><span class="sxs-lookup"><span data-stu-id="fb749-114">idToken</span></span>|<span data-ttu-id="fb749-115">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb749-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="fb749-116">JWT ID 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fb749-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="fb749-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="fb749-117">accessToken</span></span>|<span data-ttu-id="fb749-118">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb749-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="fb749-119">JWT 访问令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fb749-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="fb749-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="fb749-120">saml2Token</span></span>|<span data-ttu-id="fb749-121">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb749-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="fb749-122">SAML 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="fb749-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb749-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb749-123">JSON Representation</span></span>
<span data-ttu-id="fb749-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb749-124">Here is a JSON representation of the resource.</span></span>
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
