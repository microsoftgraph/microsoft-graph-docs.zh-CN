---
title: web 资源类型
description: 指定 web 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: 281a3f23dd0e22cae6b3ca2b67e2e9cd8b400740
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572715"
---
# <a name="web-resource-type"></a><span data-ttu-id="9114b-103">web 资源类型</span><span class="sxs-lookup"><span data-stu-id="9114b-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9114b-104">指定 web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="9114b-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="9114b-105">属性</span><span class="sxs-lookup"><span data-stu-id="9114b-105">Properties</span></span>

| <span data-ttu-id="9114b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9114b-106">Property</span></span> | <span data-ttu-id="9114b-107">类型</span><span class="sxs-lookup"><span data-stu-id="9114b-107">Type</span></span> | <span data-ttu-id="9114b-108">说明</span><span class="sxs-lookup"><span data-stu-id="9114b-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="9114b-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="9114b-109">implicitGrantSettings</span></span>|[<span data-ttu-id="9114b-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="9114b-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="9114b-111">指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。</span><span class="sxs-lookup"><span data-stu-id="9114b-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="9114b-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="9114b-112">logoutUrl</span></span>|<span data-ttu-id="9114b-113">String</span><span class="sxs-lookup"><span data-stu-id="9114b-113">String</span></span>| <span data-ttu-id="9114b-114">指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。</span><span class="sxs-lookup"><span data-stu-id="9114b-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="9114b-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="9114b-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="9114b-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="9114b-116">Boolean</span></span>| <span data-ttu-id="9114b-117">已弃用。</span><span class="sxs-lookup"><span data-stu-id="9114b-117">Deprecated.</span></span> <span data-ttu-id="9114b-118">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="9114b-118">Do not use.</span></span> | 
|<span data-ttu-id="9114b-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="9114b-119">redirectUris</span></span>|<span data-ttu-id="9114b-120">String 集合</span><span class="sxs-lookup"><span data-stu-id="9114b-120">String collection</span></span>| <span data-ttu-id="9114b-121">指定用于登录，用户令牌发送到的 Url 或 Uri 的 OAuth 2.0 授权代码和访问令牌发送到的重定向。</span><span class="sxs-lookup"><span data-stu-id="9114b-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9114b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9114b-122">JSON representation</span></span>
<span data-ttu-id="9114b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9114b-123">Here is a JSON representation of the resource.</span></span>

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
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/web.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
