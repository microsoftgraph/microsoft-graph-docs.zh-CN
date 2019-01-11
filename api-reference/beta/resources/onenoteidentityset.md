---
title: oneNoteIdentitySet 资源类型
description: '**即将提供的支持**'
localization_priority: Normal
ms.openlocfilehash: d2969d073503a9fd586641abeb3d82f719db8545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874085"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="03859-103">oneNoteIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="03859-103">oneNoteIdentitySet resource type</span></span>

> <span data-ttu-id="03859-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03859-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03859-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03859-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03859-106">**即将提供的支持**</span><span class="sxs-lookup"><span data-stu-id="03859-106">**Support coming soon**</span></span>

<span data-ttu-id="03859-107">OneNoteIdentitySet 类型是键的[OneNoteIdentity](onenoteidentity.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="03859-107">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="03859-108">它用于表示一套与各种事件关联的_笔记本_、_节_或_页_上，如_创建_或_上次修改者_的标识。</span><span class="sxs-lookup"><span data-stu-id="03859-108">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="03859-109">当前，它包含单个键_**用户**_。</span><span class="sxs-lookup"><span data-stu-id="03859-109">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="03859-110">在将来，可能添加键如设备或应用程序更改的项。</span><span class="sxs-lookup"><span data-stu-id="03859-110">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="03859-111">将在将来，与[IdentitySet](identityset.md)合并此类型</span><span class="sxs-lookup"><span data-stu-id="03859-111">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="03859-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03859-112">JSON representation</span></span>

<span data-ttu-id="03859-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03859-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="03859-114">属性</span><span class="sxs-lookup"><span data-stu-id="03859-114">Properties</span></span>
| <span data-ttu-id="03859-115">属性</span><span class="sxs-lookup"><span data-stu-id="03859-115">Property</span></span>     | <span data-ttu-id="03859-116">类型</span><span class="sxs-lookup"><span data-stu-id="03859-116">Type</span></span>   |<span data-ttu-id="03859-117">Description</span><span class="sxs-lookup"><span data-stu-id="03859-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03859-118">user</span><span class="sxs-lookup"><span data-stu-id="03859-118">user</span></span>|[<span data-ttu-id="03859-119">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="03859-119">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="03859-120">表示用户 OneNoteIdentity 资源。</span><span class="sxs-lookup"><span data-stu-id="03859-120">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
