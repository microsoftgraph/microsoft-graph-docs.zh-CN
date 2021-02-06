---
title: keyValue 资源类型
description: 提供有关登录请求的其他相关信息
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3459f827f35049b383e732c805d61371577b2260
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135392"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="09fa7-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="09fa7-103">keyValue resource type</span></span>

<span data-ttu-id="09fa7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09fa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09fa7-105">提供其他身份验证处理信息，例如服务器名称和登录和域提示的存在。</span><span class="sxs-lookup"><span data-stu-id="09fa7-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="09fa7-106">属性</span><span class="sxs-lookup"><span data-stu-id="09fa7-106">Properties</span></span>

| <span data-ttu-id="09fa7-107">属性</span><span class="sxs-lookup"><span data-stu-id="09fa7-107">Property</span></span>     | <span data-ttu-id="09fa7-108">类型</span><span class="sxs-lookup"><span data-stu-id="09fa7-108">Type</span></span>        | <span data-ttu-id="09fa7-109">说明</span><span class="sxs-lookup"><span data-stu-id="09fa7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09fa7-110">Key</span><span class="sxs-lookup"><span data-stu-id="09fa7-110">key</span></span>|<span data-ttu-id="09fa7-111">字符串</span><span class="sxs-lookup"><span data-stu-id="09fa7-111">String</span></span>|<span data-ttu-id="09fa7-112">包含与值关联的字段的名称。</span><span class="sxs-lookup"><span data-stu-id="09fa7-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="09fa7-113">当登录请求中包含登录或域提示时，相应的字段会作为键值对包含在内。</span><span class="sxs-lookup"><span data-stu-id="09fa7-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="09fa7-114">可能的键： `Login hint present` `Domain hint present` ， 。</span><span class="sxs-lookup"><span data-stu-id="09fa7-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="09fa7-115">value</span><span class="sxs-lookup"><span data-stu-id="09fa7-115">value</span></span>|<span data-ttu-id="09fa7-116">String</span><span class="sxs-lookup"><span data-stu-id="09fa7-116">String</span></span>|<span data-ttu-id="09fa7-117">包含指定键的相应值。</span><span class="sxs-lookup"><span data-stu-id="09fa7-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="09fa7-118">该值是登录请求中是否包含登录提示;否则 `true` `false` 。</span><span class="sxs-lookup"><span data-stu-id="09fa7-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="09fa7-119">该值是 `true` 域提示是否包含在登录请求中;否则 `false` 。</span><span class="sxs-lookup"><span data-stu-id="09fa7-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09fa7-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09fa7-120">JSON representation</span></span>

<span data-ttu-id="09fa7-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09fa7-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue",
  "baseType": null
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


