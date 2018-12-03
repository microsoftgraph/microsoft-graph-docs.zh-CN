---
title: synchronizationError 资源类型
description: 代表同步过程中发生的错误。
ms.openlocfilehash: a1e3725151a4e36772cd3b6079f787370f4c85dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042249"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="0b5ef-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b5ef-103">synchronizationError resource type</span></span>

> <span data-ttu-id="0b5ef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b5ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b5ef-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b5ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b5ef-106">代表同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="0b5ef-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="0b5ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b5ef-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="0b5ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b5ef-108">Property</span></span>     | <span data-ttu-id="0b5ef-109">类型</span><span class="sxs-lookup"><span data-stu-id="0b5ef-109">Type</span></span>   |<span data-ttu-id="0b5ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b5ef-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b5ef-111">code</span><span class="sxs-lookup"><span data-stu-id="0b5ef-111">code</span></span>|<span data-ttu-id="0b5ef-112">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5ef-112">String</span></span>||
|<span data-ttu-id="0b5ef-113">message</span><span class="sxs-lookup"><span data-stu-id="0b5ef-113">message</span></span>|<span data-ttu-id="0b5ef-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0b5ef-114">String</span></span>||
|<span data-ttu-id="0b5ef-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="0b5ef-115">tenantActionable</span></span>|<span data-ttu-id="0b5ef-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="0b5ef-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="0b5ef-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b5ef-117">JSON representation</span></span>

<span data-ttu-id="0b5ef-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b5ef-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->