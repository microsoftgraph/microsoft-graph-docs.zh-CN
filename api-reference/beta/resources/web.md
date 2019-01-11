---
title: web 资源类型
description: 指定 web 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: 26efe59eda739597e7193fa1ff79443f3d64b5a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890200"
---
# <a name="web-resource-type"></a><span data-ttu-id="03563-103">web 资源类型</span><span class="sxs-lookup"><span data-stu-id="03563-103">web resource type</span></span>

> <span data-ttu-id="03563-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03563-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03563-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03563-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03563-106">指定 web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="03563-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="03563-107">属性</span><span class="sxs-lookup"><span data-stu-id="03563-107">Properties</span></span>

| <span data-ttu-id="03563-108">属性</span><span class="sxs-lookup"><span data-stu-id="03563-108">Property</span></span> | <span data-ttu-id="03563-109">类型</span><span class="sxs-lookup"><span data-stu-id="03563-109">Type</span></span> | <span data-ttu-id="03563-110">Description</span><span class="sxs-lookup"><span data-stu-id="03563-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="03563-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="03563-111">implicitGrantSettings</span></span>|[<span data-ttu-id="03563-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="03563-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="03563-113">指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。</span><span class="sxs-lookup"><span data-stu-id="03563-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="03563-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="03563-114">logoutUrl</span></span>|<span data-ttu-id="03563-115">字符串</span><span class="sxs-lookup"><span data-stu-id="03563-115">String</span></span>| <span data-ttu-id="03563-116">指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。</span><span class="sxs-lookup"><span data-stu-id="03563-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="03563-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="03563-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="03563-118">布尔</span><span class="sxs-lookup"><span data-stu-id="03563-118">Boolean</span></span>| <span data-ttu-id="03563-119">已弃用。</span><span class="sxs-lookup"><span data-stu-id="03563-119">Deprecated.</span></span> <span data-ttu-id="03563-120">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="03563-120">Do not use.</span></span> | 
|<span data-ttu-id="03563-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="03563-121">redirectUris</span></span>|<span data-ttu-id="03563-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="03563-122">String collection</span></span>| <span data-ttu-id="03563-123">指定用于登录，用户令牌发送到的 Url 或 Uri 的 OAuth 2.0 授权代码和访问令牌发送到的重定向。</span><span class="sxs-lookup"><span data-stu-id="03563-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03563-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03563-124">JSON representation</span></span>
<span data-ttu-id="03563-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03563-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.web"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
