---
title: teamClassSettings 资源类型
description: 表示特定于类型为 "类" 的团队的设置。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8d345cd229c4a6c003c87865b5aaddf01096b4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998614"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="73604-103">teamClassSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="73604-103">teamClassSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73604-104">表示[团队](team.md)的特定于类的属性。</span><span class="sxs-lookup"><span data-stu-id="73604-104">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="73604-105">仅在团队表示类时可用。</span><span class="sxs-lookup"><span data-stu-id="73604-105">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="73604-106">属性</span><span class="sxs-lookup"><span data-stu-id="73604-106">Properties</span></span>
| <span data-ttu-id="73604-107">属性</span><span class="sxs-lookup"><span data-stu-id="73604-107">Property</span></span>     | <span data-ttu-id="73604-108">类型</span><span class="sxs-lookup"><span data-stu-id="73604-108">Type</span></span>   |<span data-ttu-id="73604-109">说明</span><span class="sxs-lookup"><span data-stu-id="73604-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73604-110">notifyGuardiansAboutAssignments</span><span class="sxs-lookup"><span data-stu-id="73604-110">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="73604-111">布尔</span><span class="sxs-lookup"><span data-stu-id="73604-111">Boolean</span></span>|<span data-ttu-id="73604-112">如果设置为`true`，则允许将每周分配摘要电子邮件发送给父/监护人，前提是租户管理员已启用全局设置。</span><span class="sxs-lookup"><span data-stu-id="73604-112">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73604-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73604-113">JSON representation</span></span>

<span data-ttu-id="73604-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73604-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
