---
title: teamworkTagMember 资源类型
description: 表示团队中应用了标记的用户。
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 73666dd19720e6d8882bb16fd90c612097e41d10
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059872"
---
# <a name="teamworktagmember-resource-type"></a><span data-ttu-id="55dfa-103">teamworkTagMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="55dfa-103">teamworkTagMember resource type</span></span>

<span data-ttu-id="55dfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55dfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55dfa-105">表示团队中应用了标记的用户。</span><span class="sxs-lookup"><span data-stu-id="55dfa-105">Represents a user in a team to whom a tag is applied.</span></span>

## <a name="methods"></a><span data-ttu-id="55dfa-106">方法</span><span class="sxs-lookup"><span data-stu-id="55dfa-106">Methods</span></span>
|<span data-ttu-id="55dfa-107">方法</span><span class="sxs-lookup"><span data-stu-id="55dfa-107">Method</span></span>|<span data-ttu-id="55dfa-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="55dfa-108">Return type</span></span>|<span data-ttu-id="55dfa-109">说明</span><span class="sxs-lookup"><span data-stu-id="55dfa-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55dfa-110">列出 teamworkTagMembers</span><span class="sxs-lookup"><span data-stu-id="55dfa-110">List teamworkTagMembers</span></span>](../api/teamworktagmember-list.md)|<span data-ttu-id="55dfa-111">**teamworkTagMember** 集合</span><span class="sxs-lookup"><span data-stu-id="55dfa-111">**teamworkTagMember** collection</span></span>|<span data-ttu-id="55dfa-112">获取团队中标准标记的成员及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="55dfa-112">Get a list of the members of a standard tag in a team and their properties.</span></span>|
|[<span data-ttu-id="55dfa-113">获取 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="55dfa-113">Get teamworkTagMember</span></span>](../api/teamworktagmember-get.md)|<span data-ttu-id="55dfa-114">**teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="55dfa-114">**teamworkTagMember**</span></span>|<span data-ttu-id="55dfa-115">获取团队中标准标记的成员的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55dfa-115">Get the properties and relationships of a member of a standard tag in a team.</span></span>|
|[<span data-ttu-id="55dfa-116">删除 teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="55dfa-116">Delete teamworkTagMember</span></span>](../api/teamworktagmember-delete.md)|<span data-ttu-id="55dfa-117">无</span><span class="sxs-lookup"><span data-stu-id="55dfa-117">None</span></span>|<span data-ttu-id="55dfa-118">从团队中的标准标记中删除成员。</span><span class="sxs-lookup"><span data-stu-id="55dfa-118">Delete a member from a standard tag in the team.</span></span>|

## <a name="properties"></a><span data-ttu-id="55dfa-119">属性</span><span class="sxs-lookup"><span data-stu-id="55dfa-119">Properties</span></span>
|<span data-ttu-id="55dfa-120">属性</span><span class="sxs-lookup"><span data-stu-id="55dfa-120">Property</span></span>|<span data-ttu-id="55dfa-121">类型</span><span class="sxs-lookup"><span data-stu-id="55dfa-121">Type</span></span>|<span data-ttu-id="55dfa-122">说明</span><span class="sxs-lookup"><span data-stu-id="55dfa-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55dfa-123">displayName</span><span class="sxs-lookup"><span data-stu-id="55dfa-123">displayName</span></span>|<span data-ttu-id="55dfa-124">String</span><span class="sxs-lookup"><span data-stu-id="55dfa-124">String</span></span>|<span data-ttu-id="55dfa-125">成员显示名称。</span><span class="sxs-lookup"><span data-stu-id="55dfa-125">The member's display name.</span></span>|
|<span data-ttu-id="55dfa-126">ID</span><span class="sxs-lookup"><span data-stu-id="55dfa-126">ID</span></span>|<span data-ttu-id="55dfa-127">String</span><span class="sxs-lookup"><span data-stu-id="55dfa-127">String</span></span>|<span data-ttu-id="55dfa-128">成员 ID。</span><span class="sxs-lookup"><span data-stu-id="55dfa-128">ID of the member.</span></span>|
|<span data-ttu-id="55dfa-129">tenantID</span><span class="sxs-lookup"><span data-stu-id="55dfa-129">tenantID</span></span>|<span data-ttu-id="55dfa-130">String</span><span class="sxs-lookup"><span data-stu-id="55dfa-130">String</span></span>|<span data-ttu-id="55dfa-131">标记成员是其中一部分的租户的 ID。</span><span class="sxs-lookup"><span data-stu-id="55dfa-131">The ID of the tenant that the tag member is a part of.</span></span>|
|<span data-ttu-id="55dfa-132">userID</span><span class="sxs-lookup"><span data-stu-id="55dfa-132">userID</span></span>|<span data-ttu-id="55dfa-133">String</span><span class="sxs-lookup"><span data-stu-id="55dfa-133">String</span></span>|<span data-ttu-id="55dfa-134">成员的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="55dfa-134">The user ID of the member.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55dfa-135">关系</span><span class="sxs-lookup"><span data-stu-id="55dfa-135">Relationships</span></span>
<span data-ttu-id="55dfa-136">无。</span><span class="sxs-lookup"><span data-stu-id="55dfa-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55dfa-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55dfa-137">JSON representation</span></span>
<span data-ttu-id="55dfa-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55dfa-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "ID",
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagMember",
  "ID": "String (Identifier)",
  "displayName": "String",
  "tenantID": "String",
  "userID": "String"
}
```

