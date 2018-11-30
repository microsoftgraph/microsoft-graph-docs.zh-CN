---
title: copyStatusModel 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8a4726715885e46208183aebe093f388a308de01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041765"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="102da-103">copyStatusModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="102da-103">copyStatusModel resource type</span></span>

> <span data-ttu-id="102da-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="102da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="102da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="102da-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="102da-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="102da-106">JSON representation</span></span>

<span data-ttu-id="102da-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="102da-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.copystatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="102da-108">属性</span><span class="sxs-lookup"><span data-stu-id="102da-108">Properties</span></span>
| <span data-ttu-id="102da-109">属性</span><span class="sxs-lookup"><span data-stu-id="102da-109">Property</span></span>     | <span data-ttu-id="102da-110">类型</span><span class="sxs-lookup"><span data-stu-id="102da-110">Type</span></span>   |<span data-ttu-id="102da-111">说明</span><span class="sxs-lookup"><span data-stu-id="102da-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="102da-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="102da-112">createdDateTime</span></span>| <span data-ttu-id="102da-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="102da-113">DateTimeOffset</span></span> ||
|<span data-ttu-id="102da-114">id</span><span class="sxs-lookup"><span data-stu-id="102da-114">id</span></span>|<span data-ttu-id="102da-115">string</span><span class="sxs-lookup"><span data-stu-id="102da-115">string</span></span>||
|<span data-ttu-id="102da-116">status</span><span class="sxs-lookup"><span data-stu-id="102da-116">status</span></span>|<span data-ttu-id="102da-117">string</span><span class="sxs-lookup"><span data-stu-id="102da-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "copyStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
