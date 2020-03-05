---
title: programControl 资源类型
description: 在 Azure AD access 评论功能中，program control 对象表示一个控件，将访问权限链接到某个程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ee374108cdebca2e6ae06ee18a245f5c9eeebf74
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521444"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="03905-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="03905-103">programControl resource type</span></span>

<span data-ttu-id="03905-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="03905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03905-105">在 Azure AD [access 评论](accessreviews-root.md)功能中，program control 对象表示一个控件，将访问权限链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="03905-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="03905-106">方法</span><span class="sxs-lookup"><span data-stu-id="03905-106">Methods</span></span>

| <span data-ttu-id="03905-107">方法</span><span class="sxs-lookup"><span data-stu-id="03905-107">Method</span></span>           | <span data-ttu-id="03905-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="03905-108">Return Type</span></span>    |<span data-ttu-id="03905-109">说明</span><span class="sxs-lookup"><span data-stu-id="03905-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03905-110">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="03905-110">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="03905-111">programControl</span><span class="sxs-lookup"><span data-stu-id="03905-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="03905-112">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="03905-112">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="03905-113">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="03905-113">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="03905-114">无。</span><span class="sxs-lookup"><span data-stu-id="03905-114">None.</span></span>   |   <span data-ttu-id="03905-115">从程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="03905-115">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="03905-116">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="03905-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="03905-117">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="03905-117">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="03905-118">列出租户中所有程序之间的控件。</span><span class="sxs-lookup"><span data-stu-id="03905-118">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="03905-119">属性</span><span class="sxs-lookup"><span data-stu-id="03905-119">Properties</span></span>
| <span data-ttu-id="03905-120">属性</span><span class="sxs-lookup"><span data-stu-id="03905-120">Property</span></span>     | <span data-ttu-id="03905-121">类型</span><span class="sxs-lookup"><span data-stu-id="03905-121">Type</span></span>   |<span data-ttu-id="03905-122">说明</span><span class="sxs-lookup"><span data-stu-id="03905-122">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="03905-123">程序和控件之间的链接的功能分配的标识符</span><span class="sxs-lookup"><span data-stu-id="03905-123">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="03905-124">此控件所属程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="03905-124">The programId of the program this control is a part of.</span></span> <span data-ttu-id="03905-125">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="03905-125">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="03905-126">控件的 controlId，特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="03905-126">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="03905-127">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="03905-127">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="03905-128">ProgramControlType 标识程序控制的类型-例如，链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="03905-128">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="03905-129">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="03905-129">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="03905-130">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="03905-130">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="03905-131">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="03905-131">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="03905-132">程序控件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03905-132">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="03905-133">userIdentity</span><span class="sxs-lookup"><span data-stu-id="03905-133">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="03905-134">创建程序控件的用户。</span><span class="sxs-lookup"><span data-stu-id="03905-134">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="03905-135">由该程序控件的访问审核作为目标的资源、组或应用程序。</span><span class="sxs-lookup"><span data-stu-id="03905-135">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="03905-136">关系</span><span class="sxs-lookup"><span data-stu-id="03905-136">Relationships</span></span>
| <span data-ttu-id="03905-137">关系</span><span class="sxs-lookup"><span data-stu-id="03905-137">Relationship</span></span> | <span data-ttu-id="03905-138">类型</span><span class="sxs-lookup"><span data-stu-id="03905-138">Type</span></span>   |<span data-ttu-id="03905-139">说明</span><span class="sxs-lookup"><span data-stu-id="03905-139">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="03905-140">主程序</span><span class="sxs-lookup"><span data-stu-id="03905-140">program</span></span>](program.md)               | <span data-ttu-id="03905-141">此控件所属的程序。</span><span class="sxs-lookup"><span data-stu-id="03905-141">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="03905-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="03905-142">See also</span></span>

| <span data-ttu-id="03905-143">方法</span><span class="sxs-lookup"><span data-stu-id="03905-143">Method</span></span>           | <span data-ttu-id="03905-144">返回类型</span><span class="sxs-lookup"><span data-stu-id="03905-144">Return Type</span></span>    |<span data-ttu-id="03905-145">说明</span><span class="sxs-lookup"><span data-stu-id="03905-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03905-146">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="03905-146">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="03905-147">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="03905-147">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="03905-148">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="03905-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="03905-149">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="03905-149">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="03905-150">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="03905-150">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="03905-151">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="03905-151">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03905-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03905-152">JSON representation</span></span>

<span data-ttu-id="03905-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03905-153">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="03905-154">ProgramResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="03905-154">The programResource complex type</span></span>

<span data-ttu-id="03905-155">程序控制对象中包含的程序资源是对作为访问评审目标的对象的引用的表示形式。</span><span class="sxs-lookup"><span data-stu-id="03905-155">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="03905-156">此类型将从`microsoft.graph.identity`继承并包含一个附加属性：</span><span class="sxs-lookup"><span data-stu-id="03905-156">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="03905-157">属性</span><span class="sxs-lookup"><span data-stu-id="03905-157">Property</span></span>     | <span data-ttu-id="03905-158">类型</span><span class="sxs-lookup"><span data-stu-id="03905-158">Type</span></span>   |<span data-ttu-id="03905-159">说明</span><span class="sxs-lookup"><span data-stu-id="03905-159">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="03905-160">资源的类型，指示它是一个组还是一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="03905-160">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="03905-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03905-161">JSON representation</span></span>

<span data-ttu-id="03905-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03905-162">Here is a JSON representation of the resource.</span></span>

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
