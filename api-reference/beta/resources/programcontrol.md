---
title: programControl 资源类型
description: 在 Azure AD 中访问审阅功能，程序 control 对象代表链接到程序访问审阅的一个控件。
localization_priority: Normal
ms.openlocfilehash: 82d9263a909fb11e688ffa6b27f0cf92601ae9e9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576554"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="4096f-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="4096f-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4096f-104">在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序控件对象表示的控件，将访问审阅链接到一个程序。</span><span class="sxs-lookup"><span data-stu-id="4096f-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="4096f-105">方法</span><span class="sxs-lookup"><span data-stu-id="4096f-105">Methods</span></span>

| <span data-ttu-id="4096f-106">方法</span><span class="sxs-lookup"><span data-stu-id="4096f-106">Method</span></span>           | <span data-ttu-id="4096f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4096f-107">Return Type</span></span>    |<span data-ttu-id="4096f-108">说明</span><span class="sxs-lookup"><span data-stu-id="4096f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4096f-109">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="4096f-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="4096f-110">programControl</span><span class="sxs-lookup"><span data-stu-id="4096f-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="4096f-111">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="4096f-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="4096f-112">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="4096f-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="4096f-113">无。</span><span class="sxs-lookup"><span data-stu-id="4096f-113">None.</span></span>   |   <span data-ttu-id="4096f-114">从某个程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="4096f-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="4096f-115">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="4096f-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="4096f-116">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="4096f-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="4096f-117">在租户中的所有程序列表控件中。</span><span class="sxs-lookup"><span data-stu-id="4096f-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="4096f-118">权限</span><span class="sxs-lookup"><span data-stu-id="4096f-118">Permissions</span></span>

|<span data-ttu-id="4096f-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4096f-119">Permission type</span></span>                        | <span data-ttu-id="4096f-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4096f-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4096f-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4096f-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="4096f-122">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4096f-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="4096f-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4096f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4096f-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="4096f-124">Not supported.</span></span> |
|<span data-ttu-id="4096f-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="4096f-125">Application</span></span>                            | <span data-ttu-id="4096f-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="4096f-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="4096f-127">属性</span><span class="sxs-lookup"><span data-stu-id="4096f-127">Properties</span></span>
| <span data-ttu-id="4096f-128">属性</span><span class="sxs-lookup"><span data-stu-id="4096f-128">Property</span></span>     | <span data-ttu-id="4096f-129">类型</span><span class="sxs-lookup"><span data-stu-id="4096f-129">Type</span></span>   |<span data-ttu-id="4096f-130">说明</span><span class="sxs-lookup"><span data-stu-id="4096f-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="4096f-131">功能指派的标识符的程序和控件之间的链接</span><span class="sxs-lookup"><span data-stu-id="4096f-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="4096f-132">程序 programId 此控件是组成部分。</span><span class="sxs-lookup"><span data-stu-id="4096f-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="4096f-133">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="4096f-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="4096f-134">控件的 controlId，尤其要指出的访问的标识符查看。</span><span class="sxs-lookup"><span data-stu-id="4096f-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="4096f-135">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="4096f-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="4096f-136">ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。</span><span class="sxs-lookup"><span data-stu-id="4096f-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="4096f-137">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="4096f-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="4096f-138">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="4096f-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="4096f-139">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="4096f-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="4096f-140">创建日期和时间的程序控制。</span><span class="sxs-lookup"><span data-stu-id="4096f-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="4096f-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="4096f-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="4096f-142">创建程序控制的用户。</span><span class="sxs-lookup"><span data-stu-id="4096f-142">The user who created the program control.</span></span>                                               |
| `resource`               | [<span data-ttu-id="4096f-143">programResource</span><span class="sxs-lookup"><span data-stu-id="4096f-143">programResource</span></span>](programresource.md)       | <span data-ttu-id="4096f-144">资源、 组或应用程序，此程序控制访问审阅的目标。</span><span class="sxs-lookup"><span data-stu-id="4096f-144">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="4096f-145">关系</span><span class="sxs-lookup"><span data-stu-id="4096f-145">Relationships</span></span>
| <span data-ttu-id="4096f-146">关系</span><span class="sxs-lookup"><span data-stu-id="4096f-146">Relationship</span></span> | <span data-ttu-id="4096f-147">类型</span><span class="sxs-lookup"><span data-stu-id="4096f-147">Type</span></span>   |<span data-ttu-id="4096f-148">说明</span><span class="sxs-lookup"><span data-stu-id="4096f-148">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="4096f-149">程序</span><span class="sxs-lookup"><span data-stu-id="4096f-149">program</span></span>](program.md)               | <span data-ttu-id="4096f-150">此控件属于该程序。</span><span class="sxs-lookup"><span data-stu-id="4096f-150">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="4096f-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4096f-151">See also</span></span>

| <span data-ttu-id="4096f-152">方法</span><span class="sxs-lookup"><span data-stu-id="4096f-152">Method</span></span>           | <span data-ttu-id="4096f-153">返回类型</span><span class="sxs-lookup"><span data-stu-id="4096f-153">Return Type</span></span>    |<span data-ttu-id="4096f-154">说明</span><span class="sxs-lookup"><span data-stu-id="4096f-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4096f-155">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="4096f-155">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="4096f-156">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="4096f-156">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="4096f-157">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="4096f-157">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4096f-158">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="4096f-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="4096f-159">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="4096f-159">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="4096f-160">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="4096f-160">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4096f-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4096f-161">JSON representation</span></span>

<span data-ttu-id="4096f-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4096f-162">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="4096f-163">ProgramResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="4096f-163">The programResource complex type</span></span>

<span data-ttu-id="4096f-164">包含程序 control 对象，该程序资源是引用的对目标的访问审阅的对象的表示形式。</span><span class="sxs-lookup"><span data-stu-id="4096f-164">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="4096f-165">此类型继承自`microsoft.graph.identity`，并且具有一个附加属性：</span><span class="sxs-lookup"><span data-stu-id="4096f-165">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="4096f-166">属性</span><span class="sxs-lookup"><span data-stu-id="4096f-166">Property</span></span>     | <span data-ttu-id="4096f-167">类型</span><span class="sxs-lookup"><span data-stu-id="4096f-167">Type</span></span>   |<span data-ttu-id="4096f-168">说明</span><span class="sxs-lookup"><span data-stu-id="4096f-168">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="4096f-169">资源，指明它一组或应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="4096f-169">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
