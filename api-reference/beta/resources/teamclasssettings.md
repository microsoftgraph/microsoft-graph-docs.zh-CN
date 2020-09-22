---
title: teamClassSettings 资源类型
description: 表示特定于类型为 "类" 的团队的设置。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97a20a312f899db5334003edb1b739bdc3b9e346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046669"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="f35f6-103">teamClassSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f35f6-103">teamClassSettings resource type</span></span>

<span data-ttu-id="f35f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f35f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35f6-105">表示 [团队](team.md)的特定于类的属性。</span><span class="sxs-lookup"><span data-stu-id="f35f6-105">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="f35f6-106">仅当团队代表班级时可用。</span><span class="sxs-lookup"><span data-stu-id="f35f6-106">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="f35f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="f35f6-107">Properties</span></span>
| <span data-ttu-id="f35f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f35f6-108">Property</span></span>     | <span data-ttu-id="f35f6-109">类型</span><span class="sxs-lookup"><span data-stu-id="f35f6-109">Type</span></span>   |<span data-ttu-id="f35f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="f35f6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f35f6-111">notifyGuardiansAboutAssignments</span><span class="sxs-lookup"><span data-stu-id="f35f6-111">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="f35f6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f35f6-112">Boolean</span></span>|<span data-ttu-id="f35f6-113">如果设置为 `true` ，则允许将每周分配摘要电子邮件发送给父/监护人，前提是租户管理员已启用全局设置。</span><span class="sxs-lookup"><span data-stu-id="f35f6-113">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f35f6-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f35f6-114">JSON representation</span></span>

<span data-ttu-id="f35f6-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f35f6-115">The following is a JSON representation of the resource.</span></span>

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


