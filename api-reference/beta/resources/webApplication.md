---
title: webApplication 资源类型
description: 指定 Web 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e57744c3825a669a9008cd05d649be0ec51b71ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964149"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="2b4fd-103">webApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b4fd-103">webApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b4fd-104">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="2b4fd-105">属性</span><span class="sxs-lookup"><span data-stu-id="2b4fd-105">Properties</span></span>

| <span data-ttu-id="2b4fd-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b4fd-106">Property</span></span> | <span data-ttu-id="2b4fd-107">类型</span><span class="sxs-lookup"><span data-stu-id="2b4fd-107">Type</span></span> | <span data-ttu-id="2b4fd-108">说明</span><span class="sxs-lookup"><span data-stu-id="2b4fd-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="2b4fd-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="2b4fd-109">implicitGrantSettings</span></span>|[<span data-ttu-id="2b4fd-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="2b4fd-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="2b4fd-111">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="2b4fd-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="2b4fd-112">logoutUrl</span></span>|<span data-ttu-id="2b4fd-113">String</span><span class="sxs-lookup"><span data-stu-id="2b4fd-113">String</span></span>| <span data-ttu-id="2b4fd-114">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="2b4fd-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="2b4fd-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="2b4fd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b4fd-116">Boolean</span></span>| <span data-ttu-id="2b4fd-117">已弃用。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-117">Deprecated.</span></span> <span data-ttu-id="2b4fd-118">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-118">Do not use.</span></span> | 
|<span data-ttu-id="2b4fd-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="2b4fd-119">redirectUris</span></span>|<span data-ttu-id="2b4fd-120">String collection</span><span class="sxs-lookup"><span data-stu-id="2b4fd-120">String collection</span></span>| <span data-ttu-id="2b4fd-121">指定向其发送用户令牌以进行登录的 Url, 或向其发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b4fd-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b4fd-122">JSON representation</span></span>
<span data-ttu-id="2b4fd-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b4fd-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
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
