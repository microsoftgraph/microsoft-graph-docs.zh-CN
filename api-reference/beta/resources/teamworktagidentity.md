---
title: teamworkTagIdentity 资源类型
description: 表示标记中的Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c0f6a8876533b2add5b63615095113f5485bfbca
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211302"
---
# <a name="teamworktagidentity-resource-type"></a><span data-ttu-id="d7f80-103">teamworkTagIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7f80-103">teamworkTagIdentity resource type</span></span>

<span data-ttu-id="d7f80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7f80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7f80-105">代表 **Microsoft Teams** 中的标记。</span><span class="sxs-lookup"><span data-stu-id="d7f80-105">Represents a **tag** in Microsoft Teams.</span></span> <span data-ttu-id="d7f80-106">标记允许用户快速连接到团队中的部分用户。</span><span class="sxs-lookup"><span data-stu-id="d7f80-106">Tags allow users to quickly connect to subset of users in a team.</span></span> <span data-ttu-id="d7f80-107">有关标记管理的详细信息，请参阅Microsoft Teams[中的管理Microsoft Teams。](/microsoftteams/manage-tags)</span><span class="sxs-lookup"><span data-stu-id="d7f80-107">For details about tag management in Microsoft Teams, see [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).</span></span>


<span data-ttu-id="d7f80-108">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="d7f80-108">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d7f80-109">属性</span><span class="sxs-lookup"><span data-stu-id="d7f80-109">Properties</span></span>
|<span data-ttu-id="d7f80-110">属性</span><span class="sxs-lookup"><span data-stu-id="d7f80-110">Property</span></span>|<span data-ttu-id="d7f80-111">类型</span><span class="sxs-lookup"><span data-stu-id="d7f80-111">Type</span></span>|<span data-ttu-id="d7f80-112">说明</span><span class="sxs-lookup"><span data-stu-id="d7f80-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f80-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d7f80-113">displayName</span></span>|<span data-ttu-id="d7f80-114">String</span><span class="sxs-lookup"><span data-stu-id="d7f80-114">String</span></span>|<span data-ttu-id="d7f80-115">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="d7f80-115">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="d7f80-116">标记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d7f80-116">Display name of the tag.</span></span>|
|<span data-ttu-id="d7f80-117">id</span><span class="sxs-lookup"><span data-stu-id="d7f80-117">id</span></span>|<span data-ttu-id="d7f80-118">String</span><span class="sxs-lookup"><span data-stu-id="d7f80-118">String</span></span>|<span data-ttu-id="d7f80-119">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="d7f80-119">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="d7f80-120">标记的 ID。</span><span class="sxs-lookup"><span data-stu-id="d7f80-120">ID of the tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7f80-121">关系</span><span class="sxs-lookup"><span data-stu-id="d7f80-121">Relationships</span></span>
<span data-ttu-id="d7f80-122">无。</span><span class="sxs-lookup"><span data-stu-id="d7f80-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7f80-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7f80-123">JSON representation</span></span>
<span data-ttu-id="d7f80-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7f80-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTagIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

