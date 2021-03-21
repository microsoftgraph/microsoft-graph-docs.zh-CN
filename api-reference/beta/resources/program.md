---
title: 程序资源类型
description: '在 Azure AD 访问评审功能中，程序是一个容器，可持有程序控件。 租户可以有一个或多个程序。  每个控件将访问评审链接到一个程序，以便更轻松地找到相关的访问评审。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: eb04c1e05c669758e282aebdcccfa4e55507e659
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960367"
---
# <a name="program-resource-type"></a><span data-ttu-id="5dfaf-105">程序资源类型</span><span class="sxs-lookup"><span data-stu-id="5dfaf-105">program resource type</span></span>

<span data-ttu-id="5dfaf-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dfaf-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dfaf-107">在 Azure AD [访问评审](accessreviews-root.md) 功能中，程序是一个容器，可持有程序控件。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="5dfaf-108">租户可以有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="5dfaf-109">每个控件将访问评审链接到一个程序，以便更轻松地找到相关的访问评审。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="5dfaf-110">每个已进行 Azure AD 访问评审的租户都有一个计划 `Default program` 。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="5dfaf-111">全局管理员可以创建其他计划，例如代表合规性计划。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="5dfaf-112">Methods</span><span class="sxs-lookup"><span data-stu-id="5dfaf-112">Methods</span></span>

| <span data-ttu-id="5dfaf-113">方法</span><span class="sxs-lookup"><span data-stu-id="5dfaf-113">Method</span></span>           | <span data-ttu-id="5dfaf-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="5dfaf-114">Return Type</span></span>    |<span data-ttu-id="5dfaf-115">说明</span><span class="sxs-lookup"><span data-stu-id="5dfaf-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5dfaf-116">创建程序</span><span class="sxs-lookup"><span data-stu-id="5dfaf-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="5dfaf-117">程序</span><span class="sxs-lookup"><span data-stu-id="5dfaf-117">program</span></span>](program.md)   |   <span data-ttu-id="5dfaf-118">创建新程序。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-118">Create a new program.</span></span>|
|[<span data-ttu-id="5dfaf-119">删除程序</span><span class="sxs-lookup"><span data-stu-id="5dfaf-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="5dfaf-120">无。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-120">None.</span></span>   |   <span data-ttu-id="5dfaf-121">删除程序。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-121">Delete a program.</span></span>|
|[<span data-ttu-id="5dfaf-122">列出程序</span><span class="sxs-lookup"><span data-stu-id="5dfaf-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="5dfaf-123">[program](program.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dfaf-123">[program](program.md) collection</span></span>|   <span data-ttu-id="5dfaf-124">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="5dfaf-125">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="5dfaf-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="5dfaf-126">[programControl](programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dfaf-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5dfaf-127">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="5dfaf-128">更新程序</span><span class="sxs-lookup"><span data-stu-id="5dfaf-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="5dfaf-129">程序</span><span class="sxs-lookup"><span data-stu-id="5dfaf-129">program</span></span>](program.md)|  <span data-ttu-id="5dfaf-130">更新程序。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="5dfaf-131">属性</span><span class="sxs-lookup"><span data-stu-id="5dfaf-131">Properties</span></span>
| <span data-ttu-id="5dfaf-132">属性</span><span class="sxs-lookup"><span data-stu-id="5dfaf-132">Property</span></span>     | <span data-ttu-id="5dfaf-133">类型</span><span class="sxs-lookup"><span data-stu-id="5dfaf-133">Type</span></span>   |<span data-ttu-id="5dfaf-134">说明</span><span class="sxs-lookup"><span data-stu-id="5dfaf-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5dfaf-135">id</span><span class="sxs-lookup"><span data-stu-id="5dfaf-135">id</span></span>                        |<span data-ttu-id="5dfaf-136">String</span><span class="sxs-lookup"><span data-stu-id="5dfaf-136">String</span></span>                              |  <span data-ttu-id="5dfaf-137">程序的功能分配标识符。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-137">The feature-assigned identifier of the program.</span></span>                    |
| <span data-ttu-id="5dfaf-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5dfaf-138">displayName</span></span>               |<span data-ttu-id="5dfaf-139">String</span><span class="sxs-lookup"><span data-stu-id="5dfaf-139">String</span></span>                              |  <span data-ttu-id="5dfaf-140">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-140">The name of the program.</span></span>  <span data-ttu-id="5dfaf-141">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-141">Required on create.</span></span>                  |
| <span data-ttu-id="5dfaf-142">说明</span><span class="sxs-lookup"><span data-stu-id="5dfaf-142">description</span></span>               |<span data-ttu-id="5dfaf-143">String</span><span class="sxs-lookup"><span data-stu-id="5dfaf-143">String</span></span>                              |  <span data-ttu-id="5dfaf-144">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-144">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="5dfaf-145">关系</span><span class="sxs-lookup"><span data-stu-id="5dfaf-145">Relationships</span></span>
| <span data-ttu-id="5dfaf-146">关系</span><span class="sxs-lookup"><span data-stu-id="5dfaf-146">Relationship</span></span> | <span data-ttu-id="5dfaf-147">类型</span><span class="sxs-lookup"><span data-stu-id="5dfaf-147">Type</span></span>   |<span data-ttu-id="5dfaf-148">说明</span><span class="sxs-lookup"><span data-stu-id="5dfaf-148">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="5dfaf-149">programControl</span><span class="sxs-lookup"><span data-stu-id="5dfaf-149">programControl</span></span>](programcontrol.md) | <span data-ttu-id="5dfaf-150">与程序关联的控件。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-150">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5dfaf-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5dfaf-151">JSON representation</span></span>

<span data-ttu-id="5dfaf-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dfaf-152">Here is a JSON representation of the resource.</span></span>

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


