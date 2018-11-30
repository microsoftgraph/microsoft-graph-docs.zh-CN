---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
ms.openlocfilehash: c6f429e353d80ea53c5f5c00ca084ae7a8a4a7c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041555"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="a19da-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a19da-103">participantInfo resource type</span></span>

> <span data-ttu-id="a19da-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a19da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a19da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a19da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a19da-106">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="a19da-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="a19da-107">属性</span><span class="sxs-lookup"><span data-stu-id="a19da-107">Properties</span></span>

| <span data-ttu-id="a19da-108">属性</span><span class="sxs-lookup"><span data-stu-id="a19da-108">Property</span></span>       | <span data-ttu-id="a19da-109">类型</span><span class="sxs-lookup"><span data-stu-id="a19da-109">Type</span></span>                          | <span data-ttu-id="a19da-110">说明</span><span class="sxs-lookup"><span data-stu-id="a19da-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="a19da-111">标识</span><span class="sxs-lookup"><span data-stu-id="a19da-111">identity</span></span>       | [<span data-ttu-id="a19da-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="a19da-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="a19da-113">与此参与者关联[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="a19da-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="a19da-114">languageId</span><span class="sxs-lookup"><span data-stu-id="a19da-114">languageId</span></span>     | <span data-ttu-id="a19da-115">字符串</span><span class="sxs-lookup"><span data-stu-id="a19da-115">String</span></span>                        | <span data-ttu-id="a19da-116">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="a19da-116">The language culture string.</span></span> |
| <span data-ttu-id="a19da-117">区域</span><span class="sxs-lookup"><span data-stu-id="a19da-117">region</span></span>         | <span data-ttu-id="a19da-118">字符串</span><span class="sxs-lookup"><span data-stu-id="a19da-118">String</span></span>                        | <span data-ttu-id="a19da-119">参与者的区域。</span><span class="sxs-lookup"><span data-stu-id="a19da-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a19da-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a19da-120">JSON representation</span></span>

<span data-ttu-id="a19da-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a19da-121">The following is a JSON representation of the resource.</span></span>

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