---
title: webApplication 资源类型
description: 指定 Web 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: af9f183011ee8774387288f8d02c4bade8352f6b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033508"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="56911-103">webApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="56911-103">webApplication resource type</span></span>

<span data-ttu-id="56911-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56911-105">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="56911-105">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="56911-106">属性</span><span class="sxs-lookup"><span data-stu-id="56911-106">Properties</span></span>

| <span data-ttu-id="56911-107">属性</span><span class="sxs-lookup"><span data-stu-id="56911-107">Property</span></span> | <span data-ttu-id="56911-108">类型</span><span class="sxs-lookup"><span data-stu-id="56911-108">Type</span></span> | <span data-ttu-id="56911-109">说明</span><span class="sxs-lookup"><span data-stu-id="56911-109">Description</span></span> |
|:---------|:-----|:------------|
| `homePageUrl` | <span data-ttu-id="56911-110">String</span><span class="sxs-lookup"><span data-stu-id="56911-110">String</span></span> | <span data-ttu-id="56911-111">应用程序的主页或登录页面。</span><span class="sxs-lookup"><span data-stu-id="56911-111">Home page or landing page of the application.</span></span> |
| `implicitGrantSettings` | [<span data-ttu-id="56911-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="56911-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="56911-113">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="56911-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> |
| `logoutUrl` | <span data-ttu-id="56911-114">String</span><span class="sxs-lookup"><span data-stu-id="56911-114">String</span></span> | <span data-ttu-id="56911-115">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="56911-115">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
| `redirectUris` | <span data-ttu-id="56911-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="56911-116">String collection</span></span> | <span data-ttu-id="56911-117">指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="56911-117">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56911-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56911-118">JSON representation</span></span>
<span data-ttu-id="56911-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56911-119">Here is a JSON representation of the resource.</span></span>

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


