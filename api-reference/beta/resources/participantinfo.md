---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
ms.openlocfilehash: 335626d1c34e2c54a86b0494e931c2da3fe283e7
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380490"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="737c8-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="737c8-103">participantInfo resource type</span></span>

> <span data-ttu-id="737c8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="737c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="737c8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="737c8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="737c8-106">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="737c8-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="737c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="737c8-107">Properties</span></span>

| <span data-ttu-id="737c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="737c8-108">Property</span></span>       | <span data-ttu-id="737c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="737c8-109">Type</span></span>                          | <span data-ttu-id="737c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="737c8-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="737c8-111">标识</span><span class="sxs-lookup"><span data-stu-id="737c8-111">identity</span></span>       | [<span data-ttu-id="737c8-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="737c8-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="737c8-113">与此参与者关联[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="737c8-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="737c8-114">languageId</span><span class="sxs-lookup"><span data-stu-id="737c8-114">languageId</span></span>     | <span data-ttu-id="737c8-115">字符串</span><span class="sxs-lookup"><span data-stu-id="737c8-115">String</span></span>                        | <span data-ttu-id="737c8-116">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="737c8-116">The language culture string.</span></span> |
| <span data-ttu-id="737c8-117">区域</span><span class="sxs-lookup"><span data-stu-id="737c8-117">region</span></span>         | <span data-ttu-id="737c8-118">字符串</span><span class="sxs-lookup"><span data-stu-id="737c8-118">String</span></span>                        | <span data-ttu-id="737c8-119">参与者的区域。</span><span class="sxs-lookup"><span data-stu-id="737c8-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="737c8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="737c8-120">JSON representation</span></span>

<span data-ttu-id="737c8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="737c8-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->