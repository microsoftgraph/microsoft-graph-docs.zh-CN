---
title: 键值资源类型
description: 提供有关登录请求的其他相关信息
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e3f85936e94da0485d62478f54eed8918967396b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442721"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="7ca08-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="7ca08-103">keyValue resource type</span></span>

<span data-ttu-id="7ca08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ca08-105">提供其他身份验证处理信息，如服务器名称和登录和域的提示的存在。</span><span class="sxs-lookup"><span data-stu-id="7ca08-105">Provides additional authentication processing information, such as the server name and the presence of hints for sign in and domain.</span></span>

## <a name="properties"></a><span data-ttu-id="7ca08-106">属性</span><span class="sxs-lookup"><span data-stu-id="7ca08-106">Properties</span></span>

| <span data-ttu-id="7ca08-107">属性</span><span class="sxs-lookup"><span data-stu-id="7ca08-107">Property</span></span>     | <span data-ttu-id="7ca08-108">类型</span><span class="sxs-lookup"><span data-stu-id="7ca08-108">Type</span></span>        | <span data-ttu-id="7ca08-109">说明</span><span class="sxs-lookup"><span data-stu-id="7ca08-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ca08-110">Key</span><span class="sxs-lookup"><span data-stu-id="7ca08-110">key</span></span>|<span data-ttu-id="7ca08-111">String</span><span class="sxs-lookup"><span data-stu-id="7ca08-111">String</span></span>|<span data-ttu-id="7ca08-112">包含与值相关联的字段的名称。</span><span class="sxs-lookup"><span data-stu-id="7ca08-112">Contains the name of the field that a value is associated with.</span></span> <span data-ttu-id="7ca08-113">当登录请求中包含登录或域提示时，相应的字段作为键值对包含。</span><span class="sxs-lookup"><span data-stu-id="7ca08-113">When a sign in or domain hint is included in the sign-in request, corresponding fields are included as key-value pairs.</span></span> <span data-ttu-id="7ca08-114">可能的键`Login hint present`： `Domain hint present`、。</span><span class="sxs-lookup"><span data-stu-id="7ca08-114">Possible keys: `Login hint present`, `Domain hint present`.</span></span>|
|<span data-ttu-id="7ca08-115">value</span><span class="sxs-lookup"><span data-stu-id="7ca08-115">value</span></span>|<span data-ttu-id="7ca08-116">String</span><span class="sxs-lookup"><span data-stu-id="7ca08-116">String</span></span>|<span data-ttu-id="7ca08-117">包含指定键的相应值。</span><span class="sxs-lookup"><span data-stu-id="7ca08-117">Contains the corresponding value for the specified key.</span></span> <span data-ttu-id="7ca08-118">如果登录请求`true`中包含登录提示，则值为; 否则为。否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="7ca08-118">The value is `true` if a sign in hint was included in the sign-in request; otherwise `false`.</span></span> <span data-ttu-id="7ca08-119">值是`true`在登录请求中包含域提示;否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="7ca08-119">The value is `true` if a domain hint was included in the sign-in request; otherwise `false`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ca08-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ca08-120">JSON representation</span></span>

<span data-ttu-id="7ca08-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ca08-121">The following is a JSON representation of the resource.</span></span>

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
