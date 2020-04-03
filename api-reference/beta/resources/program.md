---
title: 程序资源类型
description: '在 Azure AD access 评论功能中，程序是容器，保留程序控件。 一个租户可以有一个或多个程序。  每个控件都将访问审核链接到某个程序，以便更轻松地找到相关的访问评审。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: cc2ce31742cd4a02efbefebc85283c8d784ad16e
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125034"
---
# <a name="program-resource-type"></a><span data-ttu-id="80f4d-105">程序资源类型</span><span class="sxs-lookup"><span data-stu-id="80f4d-105">program resource type</span></span>

<span data-ttu-id="80f4d-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80f4d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f4d-107">在 Azure AD [access 评论](accessreviews-root.md)功能中，程序是容器，保留程序控件。</span><span class="sxs-lookup"><span data-stu-id="80f4d-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="80f4d-108">一个租户可以有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="80f4d-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="80f4d-109">每个控件都将访问审核链接到某个程序，以便更轻松地找到相关的访问评审。</span><span class="sxs-lookup"><span data-stu-id="80f4d-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="80f4d-110">每个具有 boarded Azure AD access 评审的租户都有一个程序`Default program`。</span><span class="sxs-lookup"><span data-stu-id="80f4d-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="80f4d-111">全局管理员可以创建其他程序，例如表示合规性计划。</span><span class="sxs-lookup"><span data-stu-id="80f4d-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="80f4d-112">方法</span><span class="sxs-lookup"><span data-stu-id="80f4d-112">Methods</span></span>

| <span data-ttu-id="80f4d-113">方法</span><span class="sxs-lookup"><span data-stu-id="80f4d-113">Method</span></span>           | <span data-ttu-id="80f4d-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="80f4d-114">Return Type</span></span>    |<span data-ttu-id="80f4d-115">说明</span><span class="sxs-lookup"><span data-stu-id="80f4d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80f4d-116">创建程序</span><span class="sxs-lookup"><span data-stu-id="80f4d-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="80f4d-117">主程序</span><span class="sxs-lookup"><span data-stu-id="80f4d-117">program</span></span>](program.md)   |   <span data-ttu-id="80f4d-118">创建新程序。</span><span class="sxs-lookup"><span data-stu-id="80f4d-118">Create a new program.</span></span>|
|[<span data-ttu-id="80f4d-119">删除程序</span><span class="sxs-lookup"><span data-stu-id="80f4d-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="80f4d-120">无。</span><span class="sxs-lookup"><span data-stu-id="80f4d-120">None.</span></span>   |   <span data-ttu-id="80f4d-121">删除程序。</span><span class="sxs-lookup"><span data-stu-id="80f4d-121">Delete a program.</span></span>|
|[<span data-ttu-id="80f4d-122">列出程序</span><span class="sxs-lookup"><span data-stu-id="80f4d-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="80f4d-123">[程序](program.md)集</span><span class="sxs-lookup"><span data-stu-id="80f4d-123">[program](program.md) collection</span></span>|   <span data-ttu-id="80f4d-124">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="80f4d-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="80f4d-125">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="80f4d-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="80f4d-126">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="80f4d-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="80f4d-127">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="80f4d-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="80f4d-128">更新程序</span><span class="sxs-lookup"><span data-stu-id="80f4d-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="80f4d-129">主程序</span><span class="sxs-lookup"><span data-stu-id="80f4d-129">program</span></span>](program.md)|  <span data-ttu-id="80f4d-130">更新程序。</span><span class="sxs-lookup"><span data-stu-id="80f4d-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="80f4d-131">属性</span><span class="sxs-lookup"><span data-stu-id="80f4d-131">Properties</span></span>
| <span data-ttu-id="80f4d-132">属性</span><span class="sxs-lookup"><span data-stu-id="80f4d-132">Property</span></span>     | <span data-ttu-id="80f4d-133">类型</span><span class="sxs-lookup"><span data-stu-id="80f4d-133">Type</span></span>   |<span data-ttu-id="80f4d-134">说明</span><span class="sxs-lookup"><span data-stu-id="80f4d-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="80f4d-135">功能分配的程序标识符。</span><span class="sxs-lookup"><span data-stu-id="80f4d-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="80f4d-136">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="80f4d-136">The name of the program.</span></span>  <span data-ttu-id="80f4d-137">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="80f4d-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="80f4d-138">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="80f4d-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="80f4d-139">关系</span><span class="sxs-lookup"><span data-stu-id="80f4d-139">Relationships</span></span>
| <span data-ttu-id="80f4d-140">关系</span><span class="sxs-lookup"><span data-stu-id="80f4d-140">Relationship</span></span> | <span data-ttu-id="80f4d-141">类型</span><span class="sxs-lookup"><span data-stu-id="80f4d-141">Type</span></span>   |<span data-ttu-id="80f4d-142">说明</span><span class="sxs-lookup"><span data-stu-id="80f4d-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="80f4d-143">programControl</span><span class="sxs-lookup"><span data-stu-id="80f4d-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="80f4d-144">与该程序关联的控件。</span><span class="sxs-lookup"><span data-stu-id="80f4d-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80f4d-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80f4d-145">JSON representation</span></span>

<span data-ttu-id="80f4d-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80f4d-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
