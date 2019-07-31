---
title: programControl 资源类型
description: 在 Azure AD access 评论功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16824c2ed0c053f0cc4f3a0a2903324ff1a2bf5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965633"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="8f58d-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f58d-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="8f58d-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="8f58d-105">方法</span><span class="sxs-lookup"><span data-stu-id="8f58d-105">Methods</span></span>

| <span data-ttu-id="8f58d-106">方法</span><span class="sxs-lookup"><span data-stu-id="8f58d-106">Method</span></span>           | <span data-ttu-id="8f58d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-107">Return Type</span></span>    |<span data-ttu-id="8f58d-108">说明</span><span class="sxs-lookup"><span data-stu-id="8f58d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f58d-109">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="8f58d-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="8f58d-110">programControl</span><span class="sxs-lookup"><span data-stu-id="8f58d-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="8f58d-111">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="8f58d-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="8f58d-112">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="8f58d-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="8f58d-113">无。</span><span class="sxs-lookup"><span data-stu-id="8f58d-113">None.</span></span>   |   <span data-ttu-id="8f58d-114">从程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="8f58d-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="8f58d-115">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="8f58d-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="8f58d-116">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f58d-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8f58d-117">列出租户中所有程序之间的控件。</span><span class="sxs-lookup"><span data-stu-id="8f58d-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f58d-118">属性</span><span class="sxs-lookup"><span data-stu-id="8f58d-118">Properties</span></span>
| <span data-ttu-id="8f58d-119">属性</span><span class="sxs-lookup"><span data-stu-id="8f58d-119">Property</span></span>     | <span data-ttu-id="8f58d-120">类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-120">Type</span></span>   |<span data-ttu-id="8f58d-121">说明</span><span class="sxs-lookup"><span data-stu-id="8f58d-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="8f58d-122">程序和控件之间的链接的功能分配的标识符</span><span class="sxs-lookup"><span data-stu-id="8f58d-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="8f58d-123">此控件所属程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="8f58d-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="8f58d-124">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="8f58d-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="8f58d-125">控件的 controlId, 特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="8f58d-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="8f58d-126">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="8f58d-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="8f58d-127">ProgramControlType 标识程序控制的类型-例如, 链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="8f58d-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="8f58d-128">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="8f58d-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="8f58d-129">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="8f58d-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="8f58d-130">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="8f58d-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="8f58d-131">程序控件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8f58d-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="8f58d-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="8f58d-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="8f58d-133">创建程序控件的用户。</span><span class="sxs-lookup"><span data-stu-id="8f58d-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="8f58d-134">由该程序控件的访问审核作为目标的资源、组或应用程序。</span><span class="sxs-lookup"><span data-stu-id="8f58d-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="8f58d-135">关系</span><span class="sxs-lookup"><span data-stu-id="8f58d-135">Relationships</span></span>
| <span data-ttu-id="8f58d-136">关系</span><span class="sxs-lookup"><span data-stu-id="8f58d-136">Relationship</span></span> | <span data-ttu-id="8f58d-137">类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-137">Type</span></span>   |<span data-ttu-id="8f58d-138">说明</span><span class="sxs-lookup"><span data-stu-id="8f58d-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="8f58d-139">主程序</span><span class="sxs-lookup"><span data-stu-id="8f58d-139">program</span></span>](program.md)               | <span data-ttu-id="8f58d-140">此控件所属的程序。</span><span class="sxs-lookup"><span data-stu-id="8f58d-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="8f58d-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8f58d-141">See also</span></span>

| <span data-ttu-id="8f58d-142">方法</span><span class="sxs-lookup"><span data-stu-id="8f58d-142">Method</span></span>           | <span data-ttu-id="8f58d-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-143">Return Type</span></span>    |<span data-ttu-id="8f58d-144">说明</span><span class="sxs-lookup"><span data-stu-id="8f58d-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f58d-145">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="8f58d-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="8f58d-146">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f58d-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8f58d-147">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="8f58d-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8f58d-148">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="8f58d-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="8f58d-149">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f58d-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="8f58d-150">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="8f58d-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f58d-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f58d-151">JSON representation</span></span>

<span data-ttu-id="8f58d-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f58d-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="8f58d-153">ProgramResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-153">The programResource complex type</span></span>

<span data-ttu-id="8f58d-154">程序控制对象中包含的程序资源是对作为访问评审目标的对象的引用的表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f58d-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="8f58d-155">此类型将从`microsoft.graph.identity`继承并包含一个附加属性:</span><span class="sxs-lookup"><span data-stu-id="8f58d-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="8f58d-156">属性</span><span class="sxs-lookup"><span data-stu-id="8f58d-156">Property</span></span>     | <span data-ttu-id="8f58d-157">类型</span><span class="sxs-lookup"><span data-stu-id="8f58d-157">Type</span></span>   |<span data-ttu-id="8f58d-158">说明</span><span class="sxs-lookup"><span data-stu-id="8f58d-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="8f58d-159">资源的类型, 指示它是一个组还是一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="8f58d-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="8f58d-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f58d-160">JSON representation</span></span>

<span data-ttu-id="8f58d-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f58d-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
