---
title: api 资源类型
description: 指定 Web API 应用程序的设置。
ms.openlocfilehash: b5b07ccb5a66027f9eb755754842f6e2e2ae708e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043796"
---
# <a name="api-resource-type"></a><span data-ttu-id="b42ad-103">api 资源类型</span><span class="sxs-lookup"><span data-stu-id="b42ad-103">api resource type</span></span>

> <span data-ttu-id="b42ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b42ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b42ad-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b42ad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b42ad-106">指定 Web API 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="b42ad-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="b42ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="b42ad-107">Properties</span></span>

| <span data-ttu-id="b42ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="b42ad-108">Property</span></span> | <span data-ttu-id="b42ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="b42ad-109">Type</span></span> | <span data-ttu-id="b42ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="b42ad-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b42ad-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="b42ad-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="b42ad-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b42ad-112">Int32</span></span>| <span data-ttu-id="b42ad-113">指定当前 API 资源的接受的访问令牌版本。</span><span class="sxs-lookup"><span data-stu-id="b42ad-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="b42ad-114">可能的值为 1 或 2。</span><span class="sxs-lookup"><span data-stu-id="b42ad-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="b42ad-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="b42ad-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="b42ad-116">[permissionScope](permissionscope.md)集合</span><span class="sxs-lookup"><span data-stu-id="b42ad-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="b42ad-117">客户端应用程序公开 web API （资源） 应用程序的 OAuth 2.0 权限范围的集合。</span><span class="sxs-lookup"><span data-stu-id="b42ad-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="b42ad-118">这些权限范围可能期间同意授予客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="b42ad-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b42ad-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b42ad-119">JSON representation</span></span>
<span data-ttu-id="b42ad-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b42ad-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->