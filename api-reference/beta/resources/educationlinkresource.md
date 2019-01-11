---
title: educationLinkResource 资源类型
description: EducationResource 一个子类。 此资源是链接，并且不会不具有任何其他数据与其关联。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 330e56b0be114128a6ea91f8f870f820fde74cef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863215"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="0f386-104">educationLinkResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f386-104">educationLinkResource resource type</span></span>

> <span data-ttu-id="0f386-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0f386-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f386-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f386-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f386-107">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="0f386-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="0f386-108">此资源是链接，并且不会不具有任何其他数据与其关联。</span><span class="sxs-lookup"><span data-stu-id="0f386-108">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="0f386-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f386-109">Properties</span></span>
| <span data-ttu-id="0f386-110">属性</span><span class="sxs-lookup"><span data-stu-id="0f386-110">Property</span></span>     | <span data-ttu-id="0f386-111">类型</span><span class="sxs-lookup"><span data-stu-id="0f386-111">Type</span></span>   |<span data-ttu-id="0f386-112">Description</span><span class="sxs-lookup"><span data-stu-id="0f386-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f386-113">link</span><span class="sxs-lookup"><span data-stu-id="0f386-113">link</span></span>|<span data-ttu-id="0f386-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0f386-114">String</span></span>|<span data-ttu-id="0f386-115">资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="0f386-115">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f386-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f386-116">JSON representation</span></span>

<span data-ttu-id="0f386-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f386-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
