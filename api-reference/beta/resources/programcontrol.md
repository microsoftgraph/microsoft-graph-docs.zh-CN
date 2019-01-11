---
title: programControl 资源类型
description: 在 Azure AD 中访问审阅功能，程序 control 对象代表链接到程序访问审阅的一个控件。
localization_priority: Normal
ms.openlocfilehash: ddf6e978277ca1801f9126597ac4b3561fe5bfb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817820"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="27a65-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="27a65-103">programControl resource type</span></span>

> <span data-ttu-id="27a65-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27a65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27a65-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27a65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27a65-106">在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序控件对象表示的控件，将访问审阅链接到一个程序。</span><span class="sxs-lookup"><span data-stu-id="27a65-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="27a65-107">方法</span><span class="sxs-lookup"><span data-stu-id="27a65-107">Methods</span></span>

| <span data-ttu-id="27a65-108">方法</span><span class="sxs-lookup"><span data-stu-id="27a65-108">Method</span></span>           | <span data-ttu-id="27a65-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="27a65-109">Return Type</span></span>    |<span data-ttu-id="27a65-110">说明</span><span class="sxs-lookup"><span data-stu-id="27a65-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27a65-111">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="27a65-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="27a65-112">programControl</span><span class="sxs-lookup"><span data-stu-id="27a65-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="27a65-113">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="27a65-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="27a65-114">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="27a65-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="27a65-115">无。</span><span class="sxs-lookup"><span data-stu-id="27a65-115">None.</span></span>   |   <span data-ttu-id="27a65-116">从某个程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="27a65-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="27a65-117">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="27a65-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="27a65-118">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="27a65-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="27a65-119">在租户中的所有程序列表控件中。</span><span class="sxs-lookup"><span data-stu-id="27a65-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="27a65-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="27a65-120">Permissions</span></span>

|<span data-ttu-id="27a65-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="27a65-121">Permission type</span></span>                        | <span data-ttu-id="27a65-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27a65-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="27a65-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27a65-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="27a65-124">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a65-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="27a65-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27a65-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a65-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="27a65-126">Not supported.</span></span> |
|<span data-ttu-id="27a65-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="27a65-127">Application</span></span>                            | <span data-ttu-id="27a65-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="27a65-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="27a65-129">属性</span><span class="sxs-lookup"><span data-stu-id="27a65-129">Properties</span></span>
| <span data-ttu-id="27a65-130">属性</span><span class="sxs-lookup"><span data-stu-id="27a65-130">Property</span></span>     | <span data-ttu-id="27a65-131">类型</span><span class="sxs-lookup"><span data-stu-id="27a65-131">Type</span></span>   |<span data-ttu-id="27a65-132">Description</span><span class="sxs-lookup"><span data-stu-id="27a65-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="27a65-133">功能指派的标识符的程序和控件之间的链接</span><span class="sxs-lookup"><span data-stu-id="27a65-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="27a65-134">程序 programId 此控件是组成部分。</span><span class="sxs-lookup"><span data-stu-id="27a65-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="27a65-135">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="27a65-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="27a65-136">控件的 controlId，尤其要指出的访问的标识符查看。</span><span class="sxs-lookup"><span data-stu-id="27a65-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="27a65-137">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="27a65-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="27a65-138">ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。</span><span class="sxs-lookup"><span data-stu-id="27a65-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="27a65-139">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="27a65-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="27a65-140">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="27a65-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="27a65-141">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="27a65-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="27a65-142">创建日期和时间的程序控制。</span><span class="sxs-lookup"><span data-stu-id="27a65-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="27a65-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="27a65-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="27a65-144">创建程序控制的用户。</span><span class="sxs-lookup"><span data-stu-id="27a65-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="27a65-145">资源、 组或应用程序，此程序控制访问审阅的目标。</span><span class="sxs-lookup"><span data-stu-id="27a65-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="27a65-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="27a65-146">Relationships</span></span>
| <span data-ttu-id="27a65-147">关系</span><span class="sxs-lookup"><span data-stu-id="27a65-147">Relationship</span></span> | <span data-ttu-id="27a65-148">类型</span><span class="sxs-lookup"><span data-stu-id="27a65-148">Type</span></span>   |<span data-ttu-id="27a65-149">Description</span><span class="sxs-lookup"><span data-stu-id="27a65-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="27a65-150">程序</span><span class="sxs-lookup"><span data-stu-id="27a65-150">program</span></span>](program.md)               | <span data-ttu-id="27a65-151">此控件属于该程序。</span><span class="sxs-lookup"><span data-stu-id="27a65-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="27a65-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="27a65-152">See also</span></span>

| <span data-ttu-id="27a65-153">方法</span><span class="sxs-lookup"><span data-stu-id="27a65-153">Method</span></span>           | <span data-ttu-id="27a65-154">返回类型</span><span class="sxs-lookup"><span data-stu-id="27a65-154">Return Type</span></span>    |<span data-ttu-id="27a65-155">说明</span><span class="sxs-lookup"><span data-stu-id="27a65-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27a65-156">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="27a65-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="27a65-157">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="27a65-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="27a65-158">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="27a65-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="27a65-159">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="27a65-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="27a65-160">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="27a65-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="27a65-161">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="27a65-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27a65-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27a65-162">JSON representation</span></span>

<span data-ttu-id="27a65-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27a65-163">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="27a65-164">ProgramResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="27a65-164">The programResource complex type</span></span>

<span data-ttu-id="27a65-165">包含程序 control 对象，该程序资源是引用的对目标的访问审阅的对象的表示形式。</span><span class="sxs-lookup"><span data-stu-id="27a65-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="27a65-166">此类型继承自`microsoft.graph.identity`，并且具有一个附加属性：</span><span class="sxs-lookup"><span data-stu-id="27a65-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="27a65-167">属性</span><span class="sxs-lookup"><span data-stu-id="27a65-167">Property</span></span>     | <span data-ttu-id="27a65-168">类型</span><span class="sxs-lookup"><span data-stu-id="27a65-168">Type</span></span>   |<span data-ttu-id="27a65-169">Description</span><span class="sxs-lookup"><span data-stu-id="27a65-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="27a65-170">资源，指明它一组或应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="27a65-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
