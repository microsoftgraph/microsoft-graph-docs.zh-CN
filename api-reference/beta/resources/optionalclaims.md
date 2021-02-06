---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d50b514fa29cf99f22bb42238ac9d6a66126ab53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132655"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="c7461-103">optionalClaims 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7461-103">optionalClaims resource type</span></span>

<span data-ttu-id="c7461-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7461-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7461-105">声明应用程序请求的可选声明。</span><span class="sxs-lookup"><span data-stu-id="c7461-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="c7461-106">应用程序可以配置可选声明，以在三种类型的令牌中返回 (ID 令牌、访问令牌、SAML 2 令牌) 它可以从安全令牌服务接收。</span><span class="sxs-lookup"><span data-stu-id="c7461-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="c7461-107">应用程序可以配置一组不同的可选声明，以在每个令牌类型中返回。</span><span class="sxs-lookup"><span data-stu-id="c7461-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="c7461-108">应用程序的 optionalClaims 属性 [是](application.md)**可选Claims** 对象。</span><span class="sxs-lookup"><span data-stu-id="c7461-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="c7461-109">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="c7461-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="c7461-110">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="c7461-110">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="c7461-111">属性</span><span class="sxs-lookup"><span data-stu-id="c7461-111">Properties</span></span>
| <span data-ttu-id="c7461-112">属性</span><span class="sxs-lookup"><span data-stu-id="c7461-112">Property</span></span>     | <span data-ttu-id="c7461-113">类型</span><span class="sxs-lookup"><span data-stu-id="c7461-113">Type</span></span>        | <span data-ttu-id="c7461-114">说明</span><span class="sxs-lookup"><span data-stu-id="c7461-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7461-115">idToken</span><span class="sxs-lookup"><span data-stu-id="c7461-115">idToken</span></span>|<span data-ttu-id="c7461-116">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7461-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="c7461-117">JWT ID 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="c7461-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="c7461-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="c7461-118">accessToken</span></span>|<span data-ttu-id="c7461-119">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7461-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="c7461-120">JWT 访问令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="c7461-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="c7461-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="c7461-121">saml2Token</span></span>|<span data-ttu-id="c7461-122">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7461-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="c7461-123">SAML 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="c7461-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7461-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7461-124">JSON Representation</span></span>
<span data-ttu-id="c7461-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7461-125">Here is a JSON representation of the resource.</span></span>
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
