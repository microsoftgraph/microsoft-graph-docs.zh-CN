---
title: teamClassSettings 资源类型
description: 表示特定于类类型的团队的设置。
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10ba45299a8c0d1b28b855aad3a2321930f618e9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060474"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="1504d-103">teamClassSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1504d-103">teamClassSettings resource type</span></span>

<span data-ttu-id="1504d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1504d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1504d-105">表示团队的特定于类 [的属性](team.md)。</span><span class="sxs-lookup"><span data-stu-id="1504d-105">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="1504d-106">仅当团队代表班级时可用。</span><span class="sxs-lookup"><span data-stu-id="1504d-106">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="1504d-107">属性</span><span class="sxs-lookup"><span data-stu-id="1504d-107">Properties</span></span>
| <span data-ttu-id="1504d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1504d-108">Property</span></span>     | <span data-ttu-id="1504d-109">类型</span><span class="sxs-lookup"><span data-stu-id="1504d-109">Type</span></span>   |<span data-ttu-id="1504d-110">说明</span><span class="sxs-lookup"><span data-stu-id="1504d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1504d-111">notifyGuardiansAboutAssignments</span><span class="sxs-lookup"><span data-stu-id="1504d-111">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="1504d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="1504d-112">Boolean</span></span>|<span data-ttu-id="1504d-113">如果设置为 ，则允许向家长/监护人发送每周作业摘要电子邮件，但租户管理员已全局启用 `true` 该设置。</span><span class="sxs-lookup"><span data-stu-id="1504d-113">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1504d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1504d-114">JSON representation</span></span>

<span data-ttu-id="1504d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1504d-115">The following is a JSON representation of the resource.</span></span>

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


