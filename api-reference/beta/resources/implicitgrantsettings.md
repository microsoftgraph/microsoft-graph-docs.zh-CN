---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。 单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。 若要启用隐式流，至少一个以下属性必须设置为 true。
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642763"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="491b9-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="491b9-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="491b9-106">指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。</span><span class="sxs-lookup"><span data-stu-id="491b9-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="491b9-107">单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。</span><span class="sxs-lookup"><span data-stu-id="491b9-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="491b9-108">若要启用隐式流，至少一个以下属性必须设置为 true。</span><span class="sxs-lookup"><span data-stu-id="491b9-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="491b9-109">属性</span><span class="sxs-lookup"><span data-stu-id="491b9-109">Properties</span></span>

| <span data-ttu-id="491b9-110">属性</span><span class="sxs-lookup"><span data-stu-id="491b9-110">Property</span></span> | <span data-ttu-id="491b9-111">类型</span><span class="sxs-lookup"><span data-stu-id="491b9-111">Type</span></span> | <span data-ttu-id="491b9-112">说明</span><span class="sxs-lookup"><span data-stu-id="491b9-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="491b9-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="491b9-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="491b9-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="491b9-114">Boolean</span></span> | <span data-ttu-id="491b9-115">指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="491b9-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="491b9-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="491b9-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="491b9-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="491b9-117">Boolean</span></span> | <span data-ttu-id="491b9-118">指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流访问令牌。</span><span class="sxs-lookup"><span data-stu-id="491b9-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="491b9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="491b9-119">JSON representation</span></span>
<span data-ttu-id="491b9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="491b9-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
