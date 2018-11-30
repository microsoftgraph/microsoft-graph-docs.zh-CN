---
title: keyValue 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 86f5f3c434a52c63536f36e6e7a0dbd1fabf3125
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047179"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="fa761-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa761-103">keyValue resource type</span></span>

> <span data-ttu-id="fa761-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa761-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa761-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa761-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa761-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa761-106">JSON representation</span></span>

<span data-ttu-id="fa761-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa761-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyvalue"
}-->

```json
{
  "key": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="fa761-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa761-108">Properties</span></span>
| <span data-ttu-id="fa761-109">属性</span><span class="sxs-lookup"><span data-stu-id="fa761-109">Property</span></span>     | <span data-ttu-id="fa761-110">类型</span><span class="sxs-lookup"><span data-stu-id="fa761-110">Type</span></span>   |<span data-ttu-id="fa761-111">说明</span><span class="sxs-lookup"><span data-stu-id="fa761-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa761-112">Key</span><span class="sxs-lookup"><span data-stu-id="fa761-112">key</span></span>|<span data-ttu-id="fa761-113">string</span><span class="sxs-lookup"><span data-stu-id="fa761-113">string</span></span>||
|<span data-ttu-id="fa761-114">值</span><span class="sxs-lookup"><span data-stu-id="fa761-114">value</span></span>|<span data-ttu-id="fa761-115">字符串</span><span class="sxs-lookup"><span data-stu-id="fa761-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->