---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。 单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。 若要启用隐式流，至少一个以下属性必须设置为 true。
localization_priority: Normal
ms.openlocfilehash: 82051c3605d9815fef8a0852e0ffa9075f4a6d78
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574514"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="37d67-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="37d67-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37d67-106">指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。</span><span class="sxs-lookup"><span data-stu-id="37d67-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="37d67-107">单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。</span><span class="sxs-lookup"><span data-stu-id="37d67-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="37d67-108">若要启用隐式流，至少一个以下属性必须设置为 true。</span><span class="sxs-lookup"><span data-stu-id="37d67-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="37d67-109">属性</span><span class="sxs-lookup"><span data-stu-id="37d67-109">Properties</span></span>

| <span data-ttu-id="37d67-110">属性</span><span class="sxs-lookup"><span data-stu-id="37d67-110">Property</span></span> | <span data-ttu-id="37d67-111">类型</span><span class="sxs-lookup"><span data-stu-id="37d67-111">Type</span></span> | <span data-ttu-id="37d67-112">说明</span><span class="sxs-lookup"><span data-stu-id="37d67-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="37d67-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="37d67-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="37d67-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="37d67-114">Boolean</span></span> | <span data-ttu-id="37d67-115">指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="37d67-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="37d67-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="37d67-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="37d67-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="37d67-117">Boolean</span></span> | <span data-ttu-id="37d67-118">指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流访问令牌。</span><span class="sxs-lookup"><span data-stu-id="37d67-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37d67-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37d67-119">JSON representation</span></span>
<span data-ttu-id="37d67-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37d67-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
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
