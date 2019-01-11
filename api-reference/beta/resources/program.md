---
title: 计划资源类型
description: '在 Azure AD 中访问审阅功能，程序是容器，保存程序控件。 租户可以有一个或多个程序。  每个控件链接到程序访问检查，以使其更轻松地找到相关的 access 审阅。  '
localization_priority: Normal
ms.openlocfilehash: a342fd159bba3f7e31c55ffab9a64a72353bc7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863901"
---
# <a name="program-resource-type"></a><span data-ttu-id="ada27-105">计划资源类型</span><span class="sxs-lookup"><span data-stu-id="ada27-105">program resource type</span></span>

> <span data-ttu-id="ada27-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ada27-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ada27-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ada27-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ada27-108">在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序是容器，保存程序控件。</span><span class="sxs-lookup"><span data-stu-id="ada27-108">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="ada27-109">租户可以有一个或多个程序。</span><span class="sxs-lookup"><span data-stu-id="ada27-109">A tenant can have one or more programs.</span></span>  <span data-ttu-id="ada27-110">每个控件链接到程序访问检查，以使其更轻松地找到相关的 access 审阅。</span><span class="sxs-lookup"><span data-stu-id="ada27-110">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="ada27-111">已在-boarded Azure AD 每个租户访问评论具有一个程序`Default program`。</span><span class="sxs-lookup"><span data-stu-id="ada27-111">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="ada27-112">全局管理员可以创建其他程序，例如表示法规遵从性计划。</span><span class="sxs-lookup"><span data-stu-id="ada27-112">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="ada27-113">方法</span><span class="sxs-lookup"><span data-stu-id="ada27-113">Methods</span></span>

| <span data-ttu-id="ada27-114">方法</span><span class="sxs-lookup"><span data-stu-id="ada27-114">Method</span></span>           | <span data-ttu-id="ada27-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="ada27-115">Return Type</span></span>    |<span data-ttu-id="ada27-116">说明</span><span class="sxs-lookup"><span data-stu-id="ada27-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ada27-117">创建程序</span><span class="sxs-lookup"><span data-stu-id="ada27-117">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="ada27-118">程序</span><span class="sxs-lookup"><span data-stu-id="ada27-118">program</span></span>](program.md)   |   <span data-ttu-id="ada27-119">创建一个新的程序。</span><span class="sxs-lookup"><span data-stu-id="ada27-119">Create a new program.</span></span>|
|[<span data-ttu-id="ada27-120">删除程序</span><span class="sxs-lookup"><span data-stu-id="ada27-120">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="ada27-121">无。</span><span class="sxs-lookup"><span data-stu-id="ada27-121">None.</span></span>   |   <span data-ttu-id="ada27-122">删除一个程序。</span><span class="sxs-lookup"><span data-stu-id="ada27-122">Delete a program.</span></span>|
|[<span data-ttu-id="ada27-123">列表程序</span><span class="sxs-lookup"><span data-stu-id="ada27-123">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="ada27-124">[程序](program.md)集</span><span class="sxs-lookup"><span data-stu-id="ada27-124">[program](program.md) collection</span></span>|   <span data-ttu-id="ada27-125">获取所有的程序的集合。</span><span class="sxs-lookup"><span data-stu-id="ada27-125">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="ada27-126">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="ada27-126">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="ada27-127">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="ada27-127">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="ada27-128">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="ada27-128">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ada27-129">更新程序</span><span class="sxs-lookup"><span data-stu-id="ada27-129">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="ada27-130">程序</span><span class="sxs-lookup"><span data-stu-id="ada27-130">program</span></span>](program.md)|  <span data-ttu-id="ada27-131">更新程序。</span><span class="sxs-lookup"><span data-stu-id="ada27-131">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="ada27-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="ada27-132">Permissions</span></span>

|<span data-ttu-id="ada27-133">权限类型</span><span class="sxs-lookup"><span data-stu-id="ada27-133">Permission type</span></span>                        | <span data-ttu-id="ada27-134">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ada27-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ada27-135">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ada27-135">Delegated (work or school account)</span></span>     | <span data-ttu-id="ada27-136">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada27-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="ada27-137">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ada27-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ada27-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="ada27-138">Not supported.</span></span> |
|<span data-ttu-id="ada27-139">应用程序</span><span class="sxs-lookup"><span data-stu-id="ada27-139">Application</span></span>                            | <span data-ttu-id="ada27-140">不支持。</span><span class="sxs-lookup"><span data-stu-id="ada27-140">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="ada27-141">属性</span><span class="sxs-lookup"><span data-stu-id="ada27-141">Properties</span></span>
| <span data-ttu-id="ada27-142">属性</span><span class="sxs-lookup"><span data-stu-id="ada27-142">Property</span></span>     | <span data-ttu-id="ada27-143">类型</span><span class="sxs-lookup"><span data-stu-id="ada27-143">Type</span></span>   |<span data-ttu-id="ada27-144">Description</span><span class="sxs-lookup"><span data-stu-id="ada27-144">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="ada27-145">功能分配的程序标识符。</span><span class="sxs-lookup"><span data-stu-id="ada27-145">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="ada27-146">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="ada27-146">The name of the program.</span></span>  <span data-ttu-id="ada27-147">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="ada27-147">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="ada27-148">该程序的描述。</span><span class="sxs-lookup"><span data-stu-id="ada27-148">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="ada27-149">Relationships</span><span class="sxs-lookup"><span data-stu-id="ada27-149">Relationships</span></span>
| <span data-ttu-id="ada27-150">关系</span><span class="sxs-lookup"><span data-stu-id="ada27-150">Relationship</span></span> | <span data-ttu-id="ada27-151">类型</span><span class="sxs-lookup"><span data-stu-id="ada27-151">Type</span></span>   |<span data-ttu-id="ada27-152">Description</span><span class="sxs-lookup"><span data-stu-id="ada27-152">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="ada27-153">programControl</span><span class="sxs-lookup"><span data-stu-id="ada27-153">programControl</span></span>](programcontrol.md) | <span data-ttu-id="ada27-154">程序相关联的控件。</span><span class="sxs-lookup"><span data-stu-id="ada27-154">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ada27-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ada27-155">JSON representation</span></span>

<span data-ttu-id="ada27-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ada27-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
