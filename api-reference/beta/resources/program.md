---
title: 程序资源类型
description: '在 Azure AD access 评论功能中, 程序是容器, 保留程序控件。 一个租户可以有一个或多个程序。  每个控件都将访问审核链接到某个程序, 以便更轻松地找到相关的访问评审。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563373"
---
# <a name="program-resource-type"></a><span data-ttu-id="b68d1-105">程序资源类型</span><span class="sxs-lookup"><span data-stu-id="b68d1-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b68d1-106">在 Azure AD [access 评论](accessreviews-root.md)功能中, 程序是容器, 保留程序控件。</span><span class="sxs-lookup"><span data-stu-id="b68d1-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="b68d1-107">一个租户可以有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="b68d1-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="b68d1-108">每个控件都将访问审核链接到某个程序, 以便更轻松地找到相关的访问评审。</span><span class="sxs-lookup"><span data-stu-id="b68d1-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="b68d1-109">每个具有 boarded Azure AD access 评审的租户都有一个程序`Default program`。</span><span class="sxs-lookup"><span data-stu-id="b68d1-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="b68d1-110">全局管理员可以创建其他程序, 例如表示合规性计划。</span><span class="sxs-lookup"><span data-stu-id="b68d1-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="b68d1-111">方法</span><span class="sxs-lookup"><span data-stu-id="b68d1-111">Methods</span></span>

| <span data-ttu-id="b68d1-112">方法</span><span class="sxs-lookup"><span data-stu-id="b68d1-112">Method</span></span>           | <span data-ttu-id="b68d1-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="b68d1-113">Return Type</span></span>    |<span data-ttu-id="b68d1-114">说明</span><span class="sxs-lookup"><span data-stu-id="b68d1-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b68d1-115">创建程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="b68d1-116">主程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-116">program</span></span>](program.md)   |   <span data-ttu-id="b68d1-117">创建新程序。</span><span class="sxs-lookup"><span data-stu-id="b68d1-117">Create a new program.</span></span>|
|[<span data-ttu-id="b68d1-118">删除程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="b68d1-119">无。</span><span class="sxs-lookup"><span data-stu-id="b68d1-119">None.</span></span>   |   <span data-ttu-id="b68d1-120">删除程序。</span><span class="sxs-lookup"><span data-stu-id="b68d1-120">Delete a program.</span></span>|
|[<span data-ttu-id="b68d1-121">列出程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="b68d1-122">[程序](program.md)集</span><span class="sxs-lookup"><span data-stu-id="b68d1-122">[program](program.md) collection</span></span>|   <span data-ttu-id="b68d1-123">获取所有程序的集合。</span><span class="sxs-lookup"><span data-stu-id="b68d1-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="b68d1-124">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="b68d1-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="b68d1-125">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="b68d1-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="b68d1-126">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="b68d1-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b68d1-127">更新程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="b68d1-128">主程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-128">program</span></span>](program.md)|  <span data-ttu-id="b68d1-129">更新程序。</span><span class="sxs-lookup"><span data-stu-id="b68d1-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="b68d1-130">权限</span><span class="sxs-lookup"><span data-stu-id="b68d1-130">Permissions</span></span>

|<span data-ttu-id="b68d1-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="b68d1-131">Permission type</span></span>                        | <span data-ttu-id="b68d1-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b68d1-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b68d1-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b68d1-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="b68d1-134">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="b68d1-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="b68d1-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b68d1-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b68d1-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="b68d1-136">Not supported.</span></span> |
|<span data-ttu-id="b68d1-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="b68d1-137">Application</span></span>                            | <span data-ttu-id="b68d1-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="b68d1-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="b68d1-139">属性</span><span class="sxs-lookup"><span data-stu-id="b68d1-139">Properties</span></span>
| <span data-ttu-id="b68d1-140">属性</span><span class="sxs-lookup"><span data-stu-id="b68d1-140">Property</span></span>     | <span data-ttu-id="b68d1-141">类型</span><span class="sxs-lookup"><span data-stu-id="b68d1-141">Type</span></span>   |<span data-ttu-id="b68d1-142">说明</span><span class="sxs-lookup"><span data-stu-id="b68d1-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="b68d1-143">功能分配的程序标识符。</span><span class="sxs-lookup"><span data-stu-id="b68d1-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="b68d1-144">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="b68d1-144">The name of the program.</span></span>  <span data-ttu-id="b68d1-145">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="b68d1-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="b68d1-146">程序的说明。</span><span class="sxs-lookup"><span data-stu-id="b68d1-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="b68d1-147">关系</span><span class="sxs-lookup"><span data-stu-id="b68d1-147">Relationships</span></span>
| <span data-ttu-id="b68d1-148">关系</span><span class="sxs-lookup"><span data-stu-id="b68d1-148">Relationship</span></span> | <span data-ttu-id="b68d1-149">类型</span><span class="sxs-lookup"><span data-stu-id="b68d1-149">Type</span></span>   |<span data-ttu-id="b68d1-150">说明</span><span class="sxs-lookup"><span data-stu-id="b68d1-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="b68d1-151">programControl</span><span class="sxs-lookup"><span data-stu-id="b68d1-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="b68d1-152">与该程序关联的控件。</span><span class="sxs-lookup"><span data-stu-id="b68d1-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b68d1-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b68d1-153">JSON representation</span></span>

<span data-ttu-id="b68d1-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b68d1-154">Here is a JSON representation of the resource.</span></span>

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
