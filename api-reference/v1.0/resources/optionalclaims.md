---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 886becff415cbc1dbaa2c5608042b0828c31c2bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939009"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="24268-103">optionalClaims 资源类型</span><span class="sxs-lookup"><span data-stu-id="24268-103">optionalClaims resource type</span></span>
<span data-ttu-id="24268-104">声明应用程序请求的可选声明。</span><span class="sxs-lookup"><span data-stu-id="24268-104">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="24268-105">应用程序可以配置可从安全令牌服务接收的三种令牌（ID 令牌、访问令牌、SAML 2 令牌）每种类型中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="24268-105">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="24268-106">应用程序可以配置要在每个令牌类型中返回的一组不同的可选声明。</span><span class="sxs-lookup"><span data-stu-id="24268-106">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="24268-107">[应用程序](application.md)的 optionalClaims 属性是一个**optionalClaims**对象。</span><span class="sxs-lookup"><span data-stu-id="24268-107">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="24268-108">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以在 Microsoft 安全令牌服务向其应用程序发送令牌中指定要使用的声明。</span><span class="sxs-lookup"><span data-stu-id="24268-108">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="24268-109">有关详细信息，请参阅向[AZURE AD 应用提供可选声明](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="24268-109">See [provide optional claims to your Azure AD app](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="24268-110">属性</span><span class="sxs-lookup"><span data-stu-id="24268-110">Properties</span></span>
| <span data-ttu-id="24268-111">属性</span><span class="sxs-lookup"><span data-stu-id="24268-111">Property</span></span>     | <span data-ttu-id="24268-112">类型</span><span class="sxs-lookup"><span data-stu-id="24268-112">Type</span></span>        | <span data-ttu-id="24268-113">描述</span><span class="sxs-lookup"><span data-stu-id="24268-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24268-114">idToken</span><span class="sxs-lookup"><span data-stu-id="24268-114">idToken</span></span>|<span data-ttu-id="24268-115">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="24268-115">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="24268-116">JWT ID 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="24268-116">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="24268-117">accessToken</span><span class="sxs-lookup"><span data-stu-id="24268-117">accessToken</span></span>|<span data-ttu-id="24268-118">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="24268-118">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="24268-119">JWT 访问令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="24268-119">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="24268-120">saml2Token</span><span class="sxs-lookup"><span data-stu-id="24268-120">saml2Token</span></span>|<span data-ttu-id="24268-121">[optionalClaim](optionalclaim.md)集合</span><span class="sxs-lookup"><span data-stu-id="24268-121">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="24268-122">SAML 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="24268-122">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24268-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24268-123">JSON Representation</span></span>
<span data-ttu-id="24268-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24268-124">Here is a JSON representation of the resource.</span></span>
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