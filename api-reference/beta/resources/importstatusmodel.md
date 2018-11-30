---
title: importStatusModel 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8174594d819803ddfe6a23e69be170bb2fdda912
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044572"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="9d386-103">importStatusModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d386-103">importStatusModel resource type</span></span>

> <span data-ttu-id="9d386-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d386-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d386-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d386-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d386-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d386-106">JSON representation</span></span>

<span data-ttu-id="9d386-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d386-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="9d386-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d386-108">Properties</span></span>
| <span data-ttu-id="9d386-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d386-109">Property</span></span>     | <span data-ttu-id="9d386-110">类型</span><span class="sxs-lookup"><span data-stu-id="9d386-110">Type</span></span>   |<span data-ttu-id="9d386-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d386-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d386-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d386-112">createdDateTime</span></span>| <span data-ttu-id="9d386-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d386-113">DateTimeOffset</span></span> ||
|<span data-ttu-id="9d386-114">id</span><span class="sxs-lookup"><span data-stu-id="9d386-114">id</span></span>|<span data-ttu-id="9d386-115">string</span><span class="sxs-lookup"><span data-stu-id="9d386-115">string</span></span>||
|<span data-ttu-id="9d386-116">status</span><span class="sxs-lookup"><span data-stu-id="9d386-116">status</span></span>|<span data-ttu-id="9d386-117">string</span><span class="sxs-lookup"><span data-stu-id="9d386-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
