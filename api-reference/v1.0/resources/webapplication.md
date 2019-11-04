---
title: webApplication 资源类型
description: 指定 Web 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c9b0c2f36913d3d89edb1bd119b2473158f0a9bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939051"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="7d2d9-103">webApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d2d9-103">webApplication resource type</span></span>

<span data-ttu-id="7d2d9-104">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="7d2d9-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="7d2d9-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d2d9-105">Properties</span></span>

| <span data-ttu-id="7d2d9-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d2d9-106">Property</span></span> | <span data-ttu-id="7d2d9-107">类型</span><span class="sxs-lookup"><span data-stu-id="7d2d9-107">Type</span></span> | <span data-ttu-id="7d2d9-108">描述</span><span class="sxs-lookup"><span data-stu-id="7d2d9-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="7d2d9-109">homePageUrl</span><span class="sxs-lookup"><span data-stu-id="7d2d9-109">homePageUrl</span></span> | <span data-ttu-id="7d2d9-110">String</span><span class="sxs-lookup"><span data-stu-id="7d2d9-110">String</span></span> | <span data-ttu-id="7d2d9-111">应用程序的主页或登录页。</span><span class="sxs-lookup"><span data-stu-id="7d2d9-111">Home page or landing page of the application.</span></span> |
| <span data-ttu-id="7d2d9-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="7d2d9-112">implicitGrantSettings</span></span> | [<span data-ttu-id="7d2d9-113">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="7d2d9-113">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="7d2d9-114">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="7d2d9-114">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| <span data-ttu-id="7d2d9-115">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="7d2d9-115">logoutUrl</span></span> | <span data-ttu-id="7d2d9-116">String</span><span class="sxs-lookup"><span data-stu-id="7d2d9-116">String</span></span> | <span data-ttu-id="7d2d9-117">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="7d2d9-117">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| <span data-ttu-id="7d2d9-118">redirectUris</span><span class="sxs-lookup"><span data-stu-id="7d2d9-118">redirectUris</span></span> | <span data-ttu-id="7d2d9-119">String collection</span><span class="sxs-lookup"><span data-stu-id="7d2d9-119">String collection</span></span> | <span data-ttu-id="7d2d9-120">指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="7d2d9-120">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d2d9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d2d9-121">JSON representation</span></span>
<span data-ttu-id="7d2d9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d2d9-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "homePageUrl": "String",
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
