---
title: programControl 资源类型
description: 在 Azure AD access 评论功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。
localization_priority: Normal
ms.openlocfilehash: 7d194f3e80f44eb57be0deb7d2ffd71624c385d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344009"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="81e44-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="81e44-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81e44-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="81e44-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="81e44-105">方法</span><span class="sxs-lookup"><span data-stu-id="81e44-105">Methods</span></span>

| <span data-ttu-id="81e44-106">方法</span><span class="sxs-lookup"><span data-stu-id="81e44-106">Method</span></span>           | <span data-ttu-id="81e44-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="81e44-107">Return Type</span></span>    |<span data-ttu-id="81e44-108">说明</span><span class="sxs-lookup"><span data-stu-id="81e44-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81e44-109">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="81e44-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="81e44-110">programControl</span><span class="sxs-lookup"><span data-stu-id="81e44-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="81e44-111">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="81e44-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="81e44-112">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="81e44-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="81e44-113">无。</span><span class="sxs-lookup"><span data-stu-id="81e44-113">None.</span></span>   |   <span data-ttu-id="81e44-114">从程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="81e44-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="81e44-115">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="81e44-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="81e44-116">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="81e44-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="81e44-117">列出租户中所有程序之间的控件。</span><span class="sxs-lookup"><span data-stu-id="81e44-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="81e44-118">属性</span><span class="sxs-lookup"><span data-stu-id="81e44-118">Properties</span></span>
| <span data-ttu-id="81e44-119">属性</span><span class="sxs-lookup"><span data-stu-id="81e44-119">Property</span></span>     | <span data-ttu-id="81e44-120">类型</span><span class="sxs-lookup"><span data-stu-id="81e44-120">Type</span></span>   |<span data-ttu-id="81e44-121">说明</span><span class="sxs-lookup"><span data-stu-id="81e44-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="81e44-122">程序和控件之间的链接的功能分配的标识符</span><span class="sxs-lookup"><span data-stu-id="81e44-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="81e44-123">此控件所属程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="81e44-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="81e44-124">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="81e44-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="81e44-125">控件的 controlId, 特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="81e44-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="81e44-126">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="81e44-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="81e44-127">programControlType 标识程序控制的类型-例如, 链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="81e44-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="81e44-128">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="81e44-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="81e44-129">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="81e44-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="81e44-130">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="81e44-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="81e44-131">程序控件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81e44-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="81e44-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="81e44-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="81e44-133">创建程序控件的用户。</span><span class="sxs-lookup"><span data-stu-id="81e44-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="81e44-134">由该程序控件的访问审核作为目标的资源、组或应用程序。</span><span class="sxs-lookup"><span data-stu-id="81e44-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="81e44-135">关系</span><span class="sxs-lookup"><span data-stu-id="81e44-135">Relationships</span></span>
| <span data-ttu-id="81e44-136">关系</span><span class="sxs-lookup"><span data-stu-id="81e44-136">Relationship</span></span> | <span data-ttu-id="81e44-137">类型</span><span class="sxs-lookup"><span data-stu-id="81e44-137">Type</span></span>   |<span data-ttu-id="81e44-138">说明</span><span class="sxs-lookup"><span data-stu-id="81e44-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="81e44-139">主程序</span><span class="sxs-lookup"><span data-stu-id="81e44-139">program</span></span>](program.md)               | <span data-ttu-id="81e44-140">此控件所属的程序。</span><span class="sxs-lookup"><span data-stu-id="81e44-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="81e44-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="81e44-141">See also</span></span>

| <span data-ttu-id="81e44-142">方法</span><span class="sxs-lookup"><span data-stu-id="81e44-142">Method</span></span>           | <span data-ttu-id="81e44-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="81e44-143">Return Type</span></span>    |<span data-ttu-id="81e44-144">说明</span><span class="sxs-lookup"><span data-stu-id="81e44-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81e44-145">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="81e44-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="81e44-146">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="81e44-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="81e44-147">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="81e44-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="81e44-148">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="81e44-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="81e44-149">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="81e44-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="81e44-150">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="81e44-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81e44-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81e44-151">JSON representation</span></span>

<span data-ttu-id="81e44-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e44-152">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="81e44-153">programResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="81e44-153">The programResource complex type</span></span>

<span data-ttu-id="81e44-154">程序控制对象中包含的程序资源是对作为访问评审目标的对象的引用的表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e44-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="81e44-155">此类型将从`microsoft.graph.identity`继承并包含一个附加属性:</span><span class="sxs-lookup"><span data-stu-id="81e44-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="81e44-156">属性</span><span class="sxs-lookup"><span data-stu-id="81e44-156">Property</span></span>     | <span data-ttu-id="81e44-157">类型</span><span class="sxs-lookup"><span data-stu-id="81e44-157">Type</span></span>   |<span data-ttu-id="81e44-158">说明</span><span class="sxs-lookup"><span data-stu-id="81e44-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="81e44-159">资源的类型, 指示它是一个组还是一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="81e44-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="81e44-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81e44-160">JSON representation</span></span>

<span data-ttu-id="81e44-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e44-161">Here is a JSON representation of the resource.</span></span>

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
