---
title: oneNoteIdentity 资源类型
description: '**即将提供的支持**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7ce71775842cc6b7084b86e13e9e4715765567ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963211"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="5e125-103">oneNoteIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e125-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="5e125-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e125-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e125-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e125-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e125-106">**即将提供的支持**</span><span class="sxs-lookup"><span data-stu-id="5e125-106">**Support coming soon**</span></span>

<span data-ttu-id="5e125-107">OneNoteIdentity 类型表示_用户_的标识。</span><span class="sxs-lookup"><span data-stu-id="5e125-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="5e125-108">将在将来，与[标识](identity.md)合并此类型</span><span class="sxs-lookup"><span data-stu-id="5e125-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e125-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e125-109">JSON representation</span></span>

<span data-ttu-id="5e125-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e125-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5e125-111">属性</span><span class="sxs-lookup"><span data-stu-id="5e125-111">Properties</span></span>
| <span data-ttu-id="5e125-112">属性</span><span class="sxs-lookup"><span data-stu-id="5e125-112">Property</span></span>     | <span data-ttu-id="5e125-113">类型</span><span class="sxs-lookup"><span data-stu-id="5e125-113">Type</span></span>   |<span data-ttu-id="5e125-114">说明</span><span class="sxs-lookup"><span data-stu-id="5e125-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e125-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5e125-115">displayName</span></span>|<span data-ttu-id="5e125-116">string</span><span class="sxs-lookup"><span data-stu-id="5e125-116">string</span></span>|<span data-ttu-id="5e125-117">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5e125-117">The identity's display name.</span></span>|
|<span data-ttu-id="5e125-118">id</span><span class="sxs-lookup"><span data-stu-id="5e125-118">id</span></span>|<span data-ttu-id="5e125-119">string</span><span class="sxs-lookup"><span data-stu-id="5e125-119">string</span></span>|<span data-ttu-id="5e125-120">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e125-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
