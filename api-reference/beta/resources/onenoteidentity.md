---
title: oneNoteIdentity 资源类型
description: '**即将提供的支持**'
ms.openlocfilehash: 09c4ee9882a420fb07c6a51be5f361b601573969
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048078"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="76668-103">oneNoteIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="76668-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="76668-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="76668-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76668-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76668-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76668-106">**即将提供的支持**</span><span class="sxs-lookup"><span data-stu-id="76668-106">**Support coming soon**</span></span>

<span data-ttu-id="76668-107">OneNoteIdentity 类型表示_用户_的标识。</span><span class="sxs-lookup"><span data-stu-id="76668-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="76668-108">将在将来，与[标识](identity.md)合并此类型</span><span class="sxs-lookup"><span data-stu-id="76668-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="76668-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76668-109">JSON representation</span></span>

<span data-ttu-id="76668-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76668-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="76668-111">属性</span><span class="sxs-lookup"><span data-stu-id="76668-111">Properties</span></span>
| <span data-ttu-id="76668-112">属性</span><span class="sxs-lookup"><span data-stu-id="76668-112">Property</span></span>     | <span data-ttu-id="76668-113">类型</span><span class="sxs-lookup"><span data-stu-id="76668-113">Type</span></span>   |<span data-ttu-id="76668-114">说明</span><span class="sxs-lookup"><span data-stu-id="76668-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76668-115">displayName</span><span class="sxs-lookup"><span data-stu-id="76668-115">displayName</span></span>|<span data-ttu-id="76668-116">string</span><span class="sxs-lookup"><span data-stu-id="76668-116">string</span></span>|<span data-ttu-id="76668-117">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="76668-117">The identity's display name.</span></span>|
|<span data-ttu-id="76668-118">id</span><span class="sxs-lookup"><span data-stu-id="76668-118">id</span></span>|<span data-ttu-id="76668-119">string</span><span class="sxs-lookup"><span data-stu-id="76668-119">string</span></span>|<span data-ttu-id="76668-120">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="76668-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
