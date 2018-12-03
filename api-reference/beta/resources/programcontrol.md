---
title: programControl 资源类型
description: 在 Azure AD 中访问审阅功能，程序 control 对象代表链接到程序访问审阅的一个控件。
ms.openlocfilehash: 03e70ffdf0607eeb11abaf1b12065b4092294d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044480"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="6a80d-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-103">programControl resource type</span></span>

> <span data-ttu-id="6a80d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a80d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a80d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a80d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a80d-106">在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序控件对象表示的控件，将访问审阅链接到一个程序。</span><span class="sxs-lookup"><span data-stu-id="6a80d-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="6a80d-107">方法</span><span class="sxs-lookup"><span data-stu-id="6a80d-107">Methods</span></span>

| <span data-ttu-id="6a80d-108">方法</span><span class="sxs-lookup"><span data-stu-id="6a80d-108">Method</span></span>           | <span data-ttu-id="6a80d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-109">Return Type</span></span>    |<span data-ttu-id="6a80d-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a80d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a80d-111">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="6a80d-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="6a80d-112">programControl</span><span class="sxs-lookup"><span data-stu-id="6a80d-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="6a80d-113">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="6a80d-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="6a80d-114">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="6a80d-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="6a80d-115">无。</span><span class="sxs-lookup"><span data-stu-id="6a80d-115">None.</span></span>   |   <span data-ttu-id="6a80d-116">从某个程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="6a80d-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="6a80d-117">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="6a80d-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="6a80d-118">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a80d-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="6a80d-119">在租户中的所有程序列表控件中。</span><span class="sxs-lookup"><span data-stu-id="6a80d-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="6a80d-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="6a80d-120">Permissions</span></span>

|<span data-ttu-id="6a80d-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-121">Permission type</span></span>                        | <span data-ttu-id="6a80d-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a80d-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a80d-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a80d-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a80d-124">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a80d-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="6a80d-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a80d-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a80d-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a80d-126">Not supported.</span></span> |
|<span data-ttu-id="6a80d-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a80d-127">Application</span></span>                            | <span data-ttu-id="6a80d-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a80d-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a80d-129">属性</span><span class="sxs-lookup"><span data-stu-id="6a80d-129">Properties</span></span>
| <span data-ttu-id="6a80d-130">属性</span><span class="sxs-lookup"><span data-stu-id="6a80d-130">Property</span></span>     | <span data-ttu-id="6a80d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-131">Type</span></span>   |<span data-ttu-id="6a80d-132">Description</span><span class="sxs-lookup"><span data-stu-id="6a80d-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="6a80d-133">功能指派的标识符的程序和控件之间的链接</span><span class="sxs-lookup"><span data-stu-id="6a80d-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="6a80d-134">程序 programId 此控件是组成部分。</span><span class="sxs-lookup"><span data-stu-id="6a80d-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="6a80d-135">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="6a80d-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="6a80d-136">控件的 controlId，尤其要指出的访问的标识符查看。</span><span class="sxs-lookup"><span data-stu-id="6a80d-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="6a80d-137">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="6a80d-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="6a80d-138">ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。</span><span class="sxs-lookup"><span data-stu-id="6a80d-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="6a80d-139">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="6a80d-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="6a80d-140">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="6a80d-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="6a80d-141">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="6a80d-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="6a80d-142">创建日期和时间的程序控制。</span><span class="sxs-lookup"><span data-stu-id="6a80d-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="6a80d-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6a80d-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="6a80d-144">创建程序控制的用户。</span><span class="sxs-lookup"><span data-stu-id="6a80d-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="6a80d-145">资源、 组或应用程序，此程序控制访问审阅的目标。</span><span class="sxs-lookup"><span data-stu-id="6a80d-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="6a80d-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="6a80d-146">Relationships</span></span>
| <span data-ttu-id="6a80d-147">关系</span><span class="sxs-lookup"><span data-stu-id="6a80d-147">Relationship</span></span> | <span data-ttu-id="6a80d-148">类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-148">Type</span></span>   |<span data-ttu-id="6a80d-149">Description</span><span class="sxs-lookup"><span data-stu-id="6a80d-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="6a80d-150">程序</span><span class="sxs-lookup"><span data-stu-id="6a80d-150">program</span></span>](program.md)               | <span data-ttu-id="6a80d-151">此控件属于该程序。</span><span class="sxs-lookup"><span data-stu-id="6a80d-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="6a80d-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6a80d-152">See also</span></span>

| <span data-ttu-id="6a80d-153">方法</span><span class="sxs-lookup"><span data-stu-id="6a80d-153">Method</span></span>           | <span data-ttu-id="6a80d-154">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-154">Return Type</span></span>    |<span data-ttu-id="6a80d-155">说明</span><span class="sxs-lookup"><span data-stu-id="6a80d-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a80d-156">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="6a80d-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="6a80d-157">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a80d-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="6a80d-158">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="6a80d-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="6a80d-159">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="6a80d-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="6a80d-160">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a80d-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="6a80d-161">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="6a80d-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a80d-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a80d-162">JSON representation</span></span>

<span data-ttu-id="6a80d-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a80d-163">Here is a JSON representation of the resource.</span></span>

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
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="6a80d-164">ProgramResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-164">The programResource complex type</span></span>

<span data-ttu-id="6a80d-165">包含程序 control 对象，该程序资源是引用的对目标的访问审阅的对象的表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a80d-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="6a80d-166">此类型继承自`microsoft.graph.identity`，并且具有一个附加属性：</span><span class="sxs-lookup"><span data-stu-id="6a80d-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="6a80d-167">属性</span><span class="sxs-lookup"><span data-stu-id="6a80d-167">Property</span></span>     | <span data-ttu-id="6a80d-168">类型</span><span class="sxs-lookup"><span data-stu-id="6a80d-168">Type</span></span>   |<span data-ttu-id="6a80d-169">Description</span><span class="sxs-lookup"><span data-stu-id="6a80d-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="6a80d-170">资源，指明它一组或应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="6a80d-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->