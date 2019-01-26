---
title: oneNoteIdentitySet 资源类型
description: '**即将提供的支持**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dc8256cb2459ae23fcdae9e2e658394df899a134
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577289"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="a781e-103">oneNoteIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="a781e-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a781e-104">**即将提供的支持**</span><span class="sxs-lookup"><span data-stu-id="a781e-104">**Support coming soon**</span></span>

<span data-ttu-id="a781e-105">OneNoteIdentitySet 类型是键的[OneNoteIdentity](onenoteidentity.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a781e-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="a781e-106">它用于表示一套与各种事件关联的_笔记本_、_节_或_页_上，如_创建_或_上次修改者_的标识。</span><span class="sxs-lookup"><span data-stu-id="a781e-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="a781e-107">当前，它包含单个键_**用户**_。</span><span class="sxs-lookup"><span data-stu-id="a781e-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="a781e-108">在将来，可能添加键如设备或应用程序更改的项。</span><span class="sxs-lookup"><span data-stu-id="a781e-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="a781e-109">将在将来，与[IdentitySet](identityset.md)合并此类型</span><span class="sxs-lookup"><span data-stu-id="a781e-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="a781e-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a781e-110">JSON representation</span></span>

<span data-ttu-id="a781e-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a781e-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oneNoteIdentitySet"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="a781e-112">属性</span><span class="sxs-lookup"><span data-stu-id="a781e-112">Properties</span></span>
| <span data-ttu-id="a781e-113">属性</span><span class="sxs-lookup"><span data-stu-id="a781e-113">Property</span></span>     | <span data-ttu-id="a781e-114">类型</span><span class="sxs-lookup"><span data-stu-id="a781e-114">Type</span></span>   |<span data-ttu-id="a781e-115">说明</span><span class="sxs-lookup"><span data-stu-id="a781e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a781e-116">user</span><span class="sxs-lookup"><span data-stu-id="a781e-116">user</span></span>|[<span data-ttu-id="a781e-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="a781e-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="a781e-118">表示用户 OneNoteIdentity 资源。</span><span class="sxs-lookup"><span data-stu-id="a781e-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
