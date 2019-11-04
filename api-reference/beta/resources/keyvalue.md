---
title: 键值资源类型
description: 提供有关登录请求的其他相关信息
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08f9fc138710626a5b8c1c2b11eeab8ed4cad673
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939304"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="03a7b-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="03a7b-103">keyValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a7b-104">提供其他身份验证处理信息，如服务器名称和登录和域的提示的存在。</span><span class="sxs-lookup"><span data-stu-id="03a7b-104">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="03a7b-105">属性</span><span class="sxs-lookup"><span data-stu-id="03a7b-105">Properties</span></span>

| <span data-ttu-id="03a7b-106">属性</span><span class="sxs-lookup"><span data-stu-id="03a7b-106">Property</span></span>     | <span data-ttu-id="03a7b-107">类型</span><span class="sxs-lookup"><span data-stu-id="03a7b-107">Type</span></span>        | <span data-ttu-id="03a7b-108">描述</span><span class="sxs-lookup"><span data-stu-id="03a7b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03a7b-109">Key</span><span class="sxs-lookup"><span data-stu-id="03a7b-109">key</span></span>|<span data-ttu-id="03a7b-110">字符串</span><span class="sxs-lookup"><span data-stu-id="03a7b-110">String</span></span>|<span data-ttu-id="03a7b-111">包含与值相关联的字段的名称。</span><span class="sxs-lookup"><span data-stu-id="03a7b-111">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="03a7b-112">当登录请求中包含登录或域提示时，相应的字段作为键值对包含。</span><span class="sxs-lookup"><span data-stu-id="03a7b-112">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="03a7b-113">可能的键`Login hint present`： `Domain hint present`、。</span><span class="sxs-lookup"><span data-stu-id="03a7b-113">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="03a7b-114">value</span><span class="sxs-lookup"><span data-stu-id="03a7b-114">value</span></span>|<span data-ttu-id="03a7b-115">String</span><span class="sxs-lookup"><span data-stu-id="03a7b-115">String</span></span>|<span data-ttu-id="03a7b-116">包含指定键的相应值。</span><span class="sxs-lookup"><span data-stu-id="03a7b-116">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="03a7b-117">如果登录请求`true`中包含登录提示，则值为; 否则为。否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="03a7b-117">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="03a7b-118">值是`true`在登录请求中包含域提示;否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="03a7b-118">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03a7b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03a7b-119">JSON representation</span></span>

<span data-ttu-id="03a7b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03a7b-120">The following is a JSON representation of the resource.</span></span>

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
