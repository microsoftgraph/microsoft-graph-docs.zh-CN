---
title: optionalClaims 类型
description: 声明应用程序请求的可选声明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: f569bf81b5af0f95bfb48a6eb9de03a09cb60a13
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998480"
---
# <a name="optionalclaims-resource-type"></a><span data-ttu-id="b8e2f-103">optionalClaims 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8e2f-103">optionalClaims resource type</span></span>

<span data-ttu-id="b8e2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8e2f-105">声明应用程序请求的可选声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-105">Declares the optional claims requested by an application.</span></span> <span data-ttu-id="b8e2f-106">应用程序可以配置可从安全令牌服务接收的三种令牌类型 (ID 令牌、访问令牌、SAML 2 令牌) 中的每种令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-106">An application can configure optional claims to be returned in each of three types of tokens (ID token, access token, SAML 2 token) it can receive from the security token service.</span></span> <span data-ttu-id="b8e2f-107">应用程序可以配置要在每个令牌类型中返回的一组不同的可选声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-107">An application can configure a different set of optional claims to be returned in each token type.</span></span> <span data-ttu-id="b8e2f-108">[应用程序](application.md)的 optionalClaims 属性是一个**optionalClaims**对象。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-108">The optionalClaims property of the [application](application.md) is an **optionalClaims** object.</span></span>

<span data-ttu-id="b8e2f-109">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-109">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="b8e2f-110">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-110">See [provide optional claims to your Azure AD app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="b8e2f-111">属性</span><span class="sxs-lookup"><span data-stu-id="b8e2f-111">Properties</span></span>
| <span data-ttu-id="b8e2f-112">属性</span><span class="sxs-lookup"><span data-stu-id="b8e2f-112">Property</span></span>     | <span data-ttu-id="b8e2f-113">类型</span><span class="sxs-lookup"><span data-stu-id="b8e2f-113">Type</span></span>        | <span data-ttu-id="b8e2f-114">说明</span><span class="sxs-lookup"><span data-stu-id="b8e2f-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8e2f-115">idToken</span><span class="sxs-lookup"><span data-stu-id="b8e2f-115">idToken</span></span>|<span data-ttu-id="b8e2f-116">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8e2f-116">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="b8e2f-117">JWT ID 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-117">The optional claims returned in the JWT ID token.</span></span> |
|<span data-ttu-id="b8e2f-118">accessToken</span><span class="sxs-lookup"><span data-stu-id="b8e2f-118">accessToken</span></span>|<span data-ttu-id="b8e2f-119">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8e2f-119">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="b8e2f-120">JWT 访问令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-120">The optional claims returned in the JWT access token.</span></span> |
|<span data-ttu-id="b8e2f-121">saml2Token</span><span class="sxs-lookup"><span data-stu-id="b8e2f-121">saml2Token</span></span>|<span data-ttu-id="b8e2f-122">[optionalClaim](optionalclaim.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8e2f-122">[optionalClaim](optionalclaim.md) collection</span></span>| <span data-ttu-id="b8e2f-123">SAML 令牌中返回的可选声明。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-123">The optional claims returned in the SAML token.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8e2f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8e2f-124">JSON Representation</span></span>
<span data-ttu-id="b8e2f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8e2f-125">Here is a JSON representation of the resource.</span></span>
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


