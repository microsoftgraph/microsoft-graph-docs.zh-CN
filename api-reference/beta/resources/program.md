---
title: 程序资源类型
description: '在 Azure AD 访问评审功能中，程序是一个包含程序控件的容器。 租户可以具有一个或多个程序。  每个控件将访问评审链接到一个程序，以便更轻松地查找相关的访问评审。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f10ee2a54a310018d87500e5dd4f939d1fe38a0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443984"
---
# <a name="program-resource-type"></a><span data-ttu-id="4f6bf-105">程序资源类型</span><span class="sxs-lookup"><span data-stu-id="4f6bf-105">program resource type</span></span>

<span data-ttu-id="4f6bf-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6bf-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f6bf-107">在 Azure AD [访问评审](accessreviews-root.md) 功能中，程序是一个包含程序控件的容器。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="4f6bf-108">租户可以具有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="4f6bf-109">每个控件将访问评审链接到一个程序，以便更轻松地查找相关的访问评审。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="4f6bf-110">每个具有已上载 Azure AD 访问评审的租户都有一个计划 `Default program` 。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="4f6bf-111">全局管理员可以创建其他计划，例如表示合规性计划。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="4f6bf-112">Methods</span><span class="sxs-lookup"><span data-stu-id="4f6bf-112">Methods</span></span>

| <span data-ttu-id="4f6bf-113">方法</span><span class="sxs-lookup"><span data-stu-id="4f6bf-113">Method</span></span>           | <span data-ttu-id="4f6bf-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f6bf-114">Return Type</span></span>    |<span data-ttu-id="4f6bf-115">说明</span><span class="sxs-lookup"><span data-stu-id="4f6bf-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f6bf-116">创建程序</span><span class="sxs-lookup"><span data-stu-id="4f6bf-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="4f6bf-117">program</span><span class="sxs-lookup"><span data-stu-id="4f6bf-117">program</span></span>](program.md)   |   <span data-ttu-id="4f6bf-118">创建新程序。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-118">Create a new program.</span></span>|
|[<span data-ttu-id="4f6bf-119">删除程序</span><span class="sxs-lookup"><span data-stu-id="4f6bf-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="4f6bf-120">无。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-120">None.</span></span>   |   <span data-ttu-id="4f6bf-121">删除程序。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-121">Delete a program.</span></span>|
|[<span data-ttu-id="4f6bf-122">列出程序</span><span class="sxs-lookup"><span data-stu-id="4f6bf-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="4f6bf-123">[program](program.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f6bf-123">[program](program.md) collection</span></span>|   <span data-ttu-id="4f6bf-124">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="4f6bf-125">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="4f6bf-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="4f6bf-126">[programControl](programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f6bf-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="4f6bf-127">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4f6bf-128">更新程序</span><span class="sxs-lookup"><span data-stu-id="4f6bf-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="4f6bf-129">program</span><span class="sxs-lookup"><span data-stu-id="4f6bf-129">program</span></span>](program.md)|  <span data-ttu-id="4f6bf-130">更新程序。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f6bf-131">属性</span><span class="sxs-lookup"><span data-stu-id="4f6bf-131">Properties</span></span>
| <span data-ttu-id="4f6bf-132">属性</span><span class="sxs-lookup"><span data-stu-id="4f6bf-132">Property</span></span>     | <span data-ttu-id="4f6bf-133">类型</span><span class="sxs-lookup"><span data-stu-id="4f6bf-133">Type</span></span>   |<span data-ttu-id="4f6bf-134">说明</span><span class="sxs-lookup"><span data-stu-id="4f6bf-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="4f6bf-135">程序的功能分配标识符。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="4f6bf-136">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-136">The name of the program.</span></span>  <span data-ttu-id="4f6bf-137">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="4f6bf-138">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="4f6bf-139">关系</span><span class="sxs-lookup"><span data-stu-id="4f6bf-139">Relationships</span></span>
| <span data-ttu-id="4f6bf-140">关系</span><span class="sxs-lookup"><span data-stu-id="4f6bf-140">Relationship</span></span> | <span data-ttu-id="4f6bf-141">类型</span><span class="sxs-lookup"><span data-stu-id="4f6bf-141">Type</span></span>   |<span data-ttu-id="4f6bf-142">说明</span><span class="sxs-lookup"><span data-stu-id="4f6bf-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="4f6bf-143">programControl</span><span class="sxs-lookup"><span data-stu-id="4f6bf-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="4f6bf-144">与程序关联的控件。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f6bf-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f6bf-145">JSON representation</span></span>

<span data-ttu-id="4f6bf-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f6bf-146">Here is a JSON representation of the resource.</span></span>

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


