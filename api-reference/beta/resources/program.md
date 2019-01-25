---
title: 计划资源类型
description: '在 Azure AD 中访问审阅功能，程序是容器，保存程序控件。 租户可以有一个或多个程序。  每个控件链接到程序访问检查，以使其更轻松地找到相关的 access 审阅。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515186"
---
# <a name="program-resource-type"></a><span data-ttu-id="6a00b-105">计划资源类型</span><span class="sxs-lookup"><span data-stu-id="6a00b-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a00b-106">在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序是容器，保存程序控件。</span><span class="sxs-lookup"><span data-stu-id="6a00b-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="6a00b-107">租户可以有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="6a00b-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="6a00b-108">每个控件链接到程序访问检查，以使其更轻松地找到相关的 access 审阅。</span><span class="sxs-lookup"><span data-stu-id="6a00b-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="6a00b-109">已在-boarded Azure AD 每个租户访问评论具有一个程序`Default program`。</span><span class="sxs-lookup"><span data-stu-id="6a00b-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="6a00b-110">全局管理员可以创建其他程序，例如表示法规遵从性计划。</span><span class="sxs-lookup"><span data-stu-id="6a00b-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="6a00b-111">方法</span><span class="sxs-lookup"><span data-stu-id="6a00b-111">Methods</span></span>

| <span data-ttu-id="6a00b-112">方法</span><span class="sxs-lookup"><span data-stu-id="6a00b-112">Method</span></span>           | <span data-ttu-id="6a00b-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a00b-113">Return Type</span></span>    |<span data-ttu-id="6a00b-114">说明</span><span class="sxs-lookup"><span data-stu-id="6a00b-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a00b-115">创建程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="6a00b-116">程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-116">program</span></span>](program.md)   |   <span data-ttu-id="6a00b-117">创建一个新的程序。</span><span class="sxs-lookup"><span data-stu-id="6a00b-117">Create a new program.</span></span>|
|[<span data-ttu-id="6a00b-118">删除程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="6a00b-119">无。</span><span class="sxs-lookup"><span data-stu-id="6a00b-119">None.</span></span>   |   <span data-ttu-id="6a00b-120">删除一个程序。</span><span class="sxs-lookup"><span data-stu-id="6a00b-120">Delete a program.</span></span>|
|[<span data-ttu-id="6a00b-121">列表程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="6a00b-122">[程序](program.md)集</span><span class="sxs-lookup"><span data-stu-id="6a00b-122">[program](program.md) collection</span></span>|   <span data-ttu-id="6a00b-123">获取所有的程序的集合。</span><span class="sxs-lookup"><span data-stu-id="6a00b-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="6a00b-124">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="6a00b-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="6a00b-125">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a00b-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="6a00b-126">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="6a00b-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="6a00b-127">更新程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="6a00b-128">程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-128">program</span></span>](program.md)|  <span data-ttu-id="6a00b-129">更新程序。</span><span class="sxs-lookup"><span data-stu-id="6a00b-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="6a00b-130">权限</span><span class="sxs-lookup"><span data-stu-id="6a00b-130">Permissions</span></span>

|<span data-ttu-id="6a00b-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a00b-131">Permission type</span></span>                        | <span data-ttu-id="6a00b-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a00b-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a00b-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a00b-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a00b-134">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a00b-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="6a00b-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a00b-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a00b-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a00b-136">Not supported.</span></span> |
|<span data-ttu-id="6a00b-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a00b-137">Application</span></span>                            | <span data-ttu-id="6a00b-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a00b-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="6a00b-139">属性</span><span class="sxs-lookup"><span data-stu-id="6a00b-139">Properties</span></span>
| <span data-ttu-id="6a00b-140">属性</span><span class="sxs-lookup"><span data-stu-id="6a00b-140">Property</span></span>     | <span data-ttu-id="6a00b-141">类型</span><span class="sxs-lookup"><span data-stu-id="6a00b-141">Type</span></span>   |<span data-ttu-id="6a00b-142">说明</span><span class="sxs-lookup"><span data-stu-id="6a00b-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="6a00b-143">功能分配的程序标识符。</span><span class="sxs-lookup"><span data-stu-id="6a00b-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="6a00b-144">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="6a00b-144">The name of the program.</span></span>  <span data-ttu-id="6a00b-145">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="6a00b-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="6a00b-146">该程序的描述。</span><span class="sxs-lookup"><span data-stu-id="6a00b-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="6a00b-147">关系</span><span class="sxs-lookup"><span data-stu-id="6a00b-147">Relationships</span></span>
| <span data-ttu-id="6a00b-148">关系</span><span class="sxs-lookup"><span data-stu-id="6a00b-148">Relationship</span></span> | <span data-ttu-id="6a00b-149">类型</span><span class="sxs-lookup"><span data-stu-id="6a00b-149">Type</span></span>   |<span data-ttu-id="6a00b-150">说明</span><span class="sxs-lookup"><span data-stu-id="6a00b-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="6a00b-151">programControl</span><span class="sxs-lookup"><span data-stu-id="6a00b-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="6a00b-152">程序相关联的控件。</span><span class="sxs-lookup"><span data-stu-id="6a00b-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a00b-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a00b-153">JSON representation</span></span>

<span data-ttu-id="6a00b-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a00b-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
