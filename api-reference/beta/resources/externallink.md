---
title: externalLink 资源类型
description: 打开 OneNote 页面或笔记本的 URL。
ms.openlocfilehash: 8f0af6b3bfd327dff0d228ea181443d742332d0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044894"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="e12ea-103">externalLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="e12ea-103">externalLink resource type</span></span>

> <span data-ttu-id="e12ea-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e12ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e12ea-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e12ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e12ea-106">打开 OneNote 页面或笔记本的 URL。</span><span class="sxs-lookup"><span data-stu-id="e12ea-106">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e12ea-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e12ea-107">JSON representation</span></span>

<span data-ttu-id="e12ea-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e12ea-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalLink"
}-->

```json
{
  "href": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e12ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="e12ea-109">Properties</span></span>
| <span data-ttu-id="e12ea-110">属性</span><span class="sxs-lookup"><span data-stu-id="e12ea-110">Property</span></span>     | <span data-ttu-id="e12ea-111">类型</span><span class="sxs-lookup"><span data-stu-id="e12ea-111">Type</span></span>   |<span data-ttu-id="e12ea-112">说明</span><span class="sxs-lookup"><span data-stu-id="e12ea-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e12ea-113">href</span><span class="sxs-lookup"><span data-stu-id="e12ea-113">href</span></span>|<span data-ttu-id="e12ea-114">String</span><span class="sxs-lookup"><span data-stu-id="e12ea-114">String</span></span>|<span data-ttu-id="e12ea-115">链接的 URL。</span><span class="sxs-lookup"><span data-stu-id="e12ea-115">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->