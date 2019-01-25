---
title: api 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521444"
---
# <a name="api-resource-type"></a><span data-ttu-id="44e5d-103">api 资源类型</span><span class="sxs-lookup"><span data-stu-id="44e5d-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44e5d-104">指定 Web API 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="44e5d-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="44e5d-105">属性</span><span class="sxs-lookup"><span data-stu-id="44e5d-105">Properties</span></span>

| <span data-ttu-id="44e5d-106">属性</span><span class="sxs-lookup"><span data-stu-id="44e5d-106">Property</span></span> | <span data-ttu-id="44e5d-107">类型</span><span class="sxs-lookup"><span data-stu-id="44e5d-107">Type</span></span> | <span data-ttu-id="44e5d-108">说明</span><span class="sxs-lookup"><span data-stu-id="44e5d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="44e5d-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="44e5d-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="44e5d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="44e5d-110">Int32</span></span>| <span data-ttu-id="44e5d-111">指定当前 API 资源的接受的访问令牌版本。</span><span class="sxs-lookup"><span data-stu-id="44e5d-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="44e5d-112">可能的值为 1 或 2。</span><span class="sxs-lookup"><span data-stu-id="44e5d-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="44e5d-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="44e5d-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="44e5d-114">[permissionScope](permissionscope.md)集合</span><span class="sxs-lookup"><span data-stu-id="44e5d-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="44e5d-115">客户端应用程序公开 web API （资源） 应用程序的 OAuth 2.0 权限范围的集合。</span><span class="sxs-lookup"><span data-stu-id="44e5d-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="44e5d-116">这些权限范围可能期间同意授予客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="44e5d-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44e5d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44e5d-117">JSON representation</span></span>
<span data-ttu-id="44e5d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44e5d-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/api.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
