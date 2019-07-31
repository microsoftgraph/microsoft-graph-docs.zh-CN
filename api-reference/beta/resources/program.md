---
title: 程序资源类型
description: '在 Azure AD access 评论功能中, 程序是容器, 保留程序控件。 一个租户可以有一个或多个程序。  每个控件都将访问审核链接到某个程序, 以便更轻松地找到相关的访问评审。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c6a978ef4bb68c09b2f5659e255d16681c9c805d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965668"
---
# <a name="program-resource-type"></a><span data-ttu-id="98909-105">程序资源类型</span><span class="sxs-lookup"><span data-stu-id="98909-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98909-106">在 Azure AD [access 评论](accessreviews-root.md)功能中, 程序是容器, 保留程序控件。</span><span class="sxs-lookup"><span data-stu-id="98909-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="98909-107">一个租户可以有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="98909-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="98909-108">每个控件都将访问审核链接到某个程序, 以便更轻松地找到相关的访问评审。</span><span class="sxs-lookup"><span data-stu-id="98909-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="98909-109">每个具有 boarded Azure AD access 评审的租户都有一个程序`Default program`。</span><span class="sxs-lookup"><span data-stu-id="98909-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="98909-110">全局管理员可以创建其他程序, 例如表示合规性计划。</span><span class="sxs-lookup"><span data-stu-id="98909-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="98909-111">方法</span><span class="sxs-lookup"><span data-stu-id="98909-111">Methods</span></span>

| <span data-ttu-id="98909-112">方法</span><span class="sxs-lookup"><span data-stu-id="98909-112">Method</span></span>           | <span data-ttu-id="98909-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="98909-113">Return Type</span></span>    |<span data-ttu-id="98909-114">说明</span><span class="sxs-lookup"><span data-stu-id="98909-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98909-115">创建程序</span><span class="sxs-lookup"><span data-stu-id="98909-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="98909-116">主程序</span><span class="sxs-lookup"><span data-stu-id="98909-116">program</span></span>](program.md)   |   <span data-ttu-id="98909-117">创建新程序。</span><span class="sxs-lookup"><span data-stu-id="98909-117">Create a new program.</span></span>|
|[<span data-ttu-id="98909-118">删除程序</span><span class="sxs-lookup"><span data-stu-id="98909-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="98909-119">无。</span><span class="sxs-lookup"><span data-stu-id="98909-119">None.</span></span>   |   <span data-ttu-id="98909-120">删除程序。</span><span class="sxs-lookup"><span data-stu-id="98909-120">Delete a program.</span></span>|
|[<span data-ttu-id="98909-121">列出程序</span><span class="sxs-lookup"><span data-stu-id="98909-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="98909-122">[程序](program.md)集</span><span class="sxs-lookup"><span data-stu-id="98909-122">[program](program.md) collection</span></span>|   <span data-ttu-id="98909-123">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="98909-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="98909-124">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="98909-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="98909-125">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="98909-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="98909-126">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="98909-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="98909-127">更新程序</span><span class="sxs-lookup"><span data-stu-id="98909-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="98909-128">主程序</span><span class="sxs-lookup"><span data-stu-id="98909-128">program</span></span>](program.md)|  <span data-ttu-id="98909-129">更新程序。</span><span class="sxs-lookup"><span data-stu-id="98909-129">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="98909-130">属性</span><span class="sxs-lookup"><span data-stu-id="98909-130">Properties</span></span>
| <span data-ttu-id="98909-131">属性</span><span class="sxs-lookup"><span data-stu-id="98909-131">Property</span></span>     | <span data-ttu-id="98909-132">类型</span><span class="sxs-lookup"><span data-stu-id="98909-132">Type</span></span>   |<span data-ttu-id="98909-133">说明</span><span class="sxs-lookup"><span data-stu-id="98909-133">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="98909-134">功能分配的程序标识符。</span><span class="sxs-lookup"><span data-stu-id="98909-134">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="98909-135">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="98909-135">The name of the program.</span></span>  <span data-ttu-id="98909-136">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="98909-136">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="98909-137">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="98909-137">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="98909-138">关系</span><span class="sxs-lookup"><span data-stu-id="98909-138">Relationships</span></span>
| <span data-ttu-id="98909-139">关系</span><span class="sxs-lookup"><span data-stu-id="98909-139">Relationship</span></span> | <span data-ttu-id="98909-140">类型</span><span class="sxs-lookup"><span data-stu-id="98909-140">Type</span></span>   |<span data-ttu-id="98909-141">说明</span><span class="sxs-lookup"><span data-stu-id="98909-141">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="98909-142">programControl</span><span class="sxs-lookup"><span data-stu-id="98909-142">programControl</span></span>](programcontrol.md) | <span data-ttu-id="98909-143">与该程序关联的控件。</span><span class="sxs-lookup"><span data-stu-id="98909-143">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98909-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98909-144">JSON representation</span></span>

<span data-ttu-id="98909-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98909-145">Here is a JSON representation of the resource.</span></span>

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
