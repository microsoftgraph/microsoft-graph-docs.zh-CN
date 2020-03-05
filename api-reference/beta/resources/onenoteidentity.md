---
title: oneNoteIdentity 资源类型
description: '**支持即将推出**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ad578dcfa54f51484aa7e29ad5c3ade8a9195b61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522356"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="aa228-103">oneNoteIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa228-103">oneNoteIdentity resource type</span></span>

<span data-ttu-id="aa228-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="aa228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa228-105">**支持即将推出**</span><span class="sxs-lookup"><span data-stu-id="aa228-105">**Support coming soon**</span></span>

<span data-ttu-id="aa228-106">OneNoteIdentity 类型表示_用户_的标识。</span><span class="sxs-lookup"><span data-stu-id="aa228-106">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="aa228-107">将来，此类型将与[标识](identity.md)合并</span><span class="sxs-lookup"><span data-stu-id="aa228-107">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="aa228-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa228-108">JSON representation</span></span>

<span data-ttu-id="aa228-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa228-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="aa228-110">属性</span><span class="sxs-lookup"><span data-stu-id="aa228-110">Properties</span></span>
| <span data-ttu-id="aa228-111">属性</span><span class="sxs-lookup"><span data-stu-id="aa228-111">Property</span></span>     | <span data-ttu-id="aa228-112">类型</span><span class="sxs-lookup"><span data-stu-id="aa228-112">Type</span></span>   |<span data-ttu-id="aa228-113">说明</span><span class="sxs-lookup"><span data-stu-id="aa228-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa228-114">displayName</span><span class="sxs-lookup"><span data-stu-id="aa228-114">displayName</span></span>|<span data-ttu-id="aa228-115">string</span><span class="sxs-lookup"><span data-stu-id="aa228-115">string</span></span>|<span data-ttu-id="aa228-116">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aa228-116">The identity's display name.</span></span>|
|<span data-ttu-id="aa228-117">id</span><span class="sxs-lookup"><span data-stu-id="aa228-117">id</span></span>|<span data-ttu-id="aa228-118">string</span><span class="sxs-lookup"><span data-stu-id="aa228-118">string</span></span>|<span data-ttu-id="aa228-119">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aa228-119">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
