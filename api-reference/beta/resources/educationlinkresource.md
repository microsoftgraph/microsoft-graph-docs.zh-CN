---
title: educationLinkResource 资源类型
description: EducationResource 一个子类。 此资源是链接，并且不会不具有任何其他数据与其关联。
author: mmast-msft
ms.openlocfilehash: 02a55eeea25ab2c27d6c5848fbc178ff535d5e33
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349801"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="e8dab-104">educationLinkResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8dab-104">educationLinkResource resource type</span></span>

> <span data-ttu-id="e8dab-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8dab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8dab-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8dab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8dab-107">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="e8dab-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="e8dab-108">此资源是链接，并且不会不具有任何其他数据与其关联。</span><span class="sxs-lookup"><span data-stu-id="e8dab-108">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="e8dab-109">属性</span><span class="sxs-lookup"><span data-stu-id="e8dab-109">Properties</span></span>
| <span data-ttu-id="e8dab-110">属性</span><span class="sxs-lookup"><span data-stu-id="e8dab-110">Property</span></span>     | <span data-ttu-id="e8dab-111">类型</span><span class="sxs-lookup"><span data-stu-id="e8dab-111">Type</span></span>   |<span data-ttu-id="e8dab-112">说明</span><span class="sxs-lookup"><span data-stu-id="e8dab-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8dab-113">link</span><span class="sxs-lookup"><span data-stu-id="e8dab-113">link</span></span>|<span data-ttu-id="e8dab-114">字符串</span><span class="sxs-lookup"><span data-stu-id="e8dab-114">String</span></span>|<span data-ttu-id="e8dab-115">资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="e8dab-115">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8dab-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8dab-116">JSON representation</span></span>

<span data-ttu-id="e8dab-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8dab-117">The following is a JSON representation of the resource.</span></span>

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