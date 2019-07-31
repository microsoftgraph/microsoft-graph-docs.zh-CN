---
title: oneNoteIdentity 资源类型
description: '**支持即将推出**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0a7df80dd3dcd4f4b93edb4e708e65de3f74d775
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966445"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="3d13d-103">oneNoteIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d13d-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d13d-104">**支持即将推出**</span><span class="sxs-lookup"><span data-stu-id="3d13d-104">**Support coming soon**</span></span>

<span data-ttu-id="3d13d-105">OneNoteIdentity 类型表示_用户_的标识。</span><span class="sxs-lookup"><span data-stu-id="3d13d-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="3d13d-106">将来, 此类型将与[标识](identity.md)合并</span><span class="sxs-lookup"><span data-stu-id="3d13d-106">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="3d13d-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d13d-107">JSON representation</span></span>

<span data-ttu-id="3d13d-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d13d-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3d13d-109">属性</span><span class="sxs-lookup"><span data-stu-id="3d13d-109">Properties</span></span>
| <span data-ttu-id="3d13d-110">属性</span><span class="sxs-lookup"><span data-stu-id="3d13d-110">Property</span></span>     | <span data-ttu-id="3d13d-111">类型</span><span class="sxs-lookup"><span data-stu-id="3d13d-111">Type</span></span>   |<span data-ttu-id="3d13d-112">说明</span><span class="sxs-lookup"><span data-stu-id="3d13d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d13d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="3d13d-113">displayName</span></span>|<span data-ttu-id="3d13d-114">string</span><span class="sxs-lookup"><span data-stu-id="3d13d-114">string</span></span>|<span data-ttu-id="3d13d-115">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3d13d-115">The identity's display name.</span></span>|
|<span data-ttu-id="3d13d-116">id</span><span class="sxs-lookup"><span data-stu-id="3d13d-116">id</span></span>|<span data-ttu-id="3d13d-117">string</span><span class="sxs-lookup"><span data-stu-id="3d13d-117">string</span></span>|<span data-ttu-id="3d13d-118">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3d13d-118">Unique identifier for the identity.</span></span>|

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
