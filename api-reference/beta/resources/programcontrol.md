---
title: programControl 资源类型
description: 在 Azure AD 中访问审阅功能，程序 control 对象代表链接到程序访问审阅的一个控件。
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511413"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="2c6e4-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c6e4-104">在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序控件对象表示的控件，将访问审阅链接到一个程序。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="2c6e4-105">方法</span><span class="sxs-lookup"><span data-stu-id="2c6e4-105">Methods</span></span>

| <span data-ttu-id="2c6e4-106">方法</span><span class="sxs-lookup"><span data-stu-id="2c6e4-106">Method</span></span>           | <span data-ttu-id="2c6e4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-107">Return Type</span></span>    |<span data-ttu-id="2c6e4-108">说明</span><span class="sxs-lookup"><span data-stu-id="2c6e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c6e4-109">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="2c6e4-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="2c6e4-110">programControl</span><span class="sxs-lookup"><span data-stu-id="2c6e4-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="2c6e4-111">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="2c6e4-112">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="2c6e4-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="2c6e4-113">无。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-113">None.</span></span>   |   <span data-ttu-id="2c6e4-114">从某个程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="2c6e4-115">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="2c6e4-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="2c6e4-116">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c6e4-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="2c6e4-117">在租户中的所有程序列表控件中。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="2c6e4-118">权限</span><span class="sxs-lookup"><span data-stu-id="2c6e4-118">Permissions</span></span>

|<span data-ttu-id="2c6e4-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-119">Permission type</span></span>                        | <span data-ttu-id="2c6e4-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c6e4-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c6e4-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c6e4-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c6e4-122">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6e4-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="2c6e4-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c6e4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c6e4-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-124">Not supported.</span></span> |
|<span data-ttu-id="2c6e4-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c6e4-125">Application</span></span>                            | <span data-ttu-id="2c6e4-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c6e4-127">属性</span><span class="sxs-lookup"><span data-stu-id="2c6e4-127">Properties</span></span>
| <span data-ttu-id="2c6e4-128">属性</span><span class="sxs-lookup"><span data-stu-id="2c6e4-128">Property</span></span>     | <span data-ttu-id="2c6e4-129">类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-129">Type</span></span>   |<span data-ttu-id="2c6e4-130">说明</span><span class="sxs-lookup"><span data-stu-id="2c6e4-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="2c6e4-131">功能指派的标识符的程序和控件之间的链接</span><span class="sxs-lookup"><span data-stu-id="2c6e4-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="2c6e4-132">程序 programId 此控件是组成部分。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="2c6e4-133">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="2c6e4-134">控件的 controlId，尤其要指出的访问的标识符查看。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="2c6e4-135">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="2c6e4-136">ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="2c6e4-137">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="2c6e4-138">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="2c6e4-139">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="2c6e4-140">创建日期和时间的程序控制。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="2c6e4-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="2c6e4-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="2c6e4-142">创建程序控制的用户。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="2c6e4-143">资源、 组或应用程序，此程序控制访问审阅的目标。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="2c6e4-144">关系</span><span class="sxs-lookup"><span data-stu-id="2c6e4-144">Relationships</span></span>
| <span data-ttu-id="2c6e4-145">关系</span><span class="sxs-lookup"><span data-stu-id="2c6e4-145">Relationship</span></span> | <span data-ttu-id="2c6e4-146">类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-146">Type</span></span>   |<span data-ttu-id="2c6e4-147">说明</span><span class="sxs-lookup"><span data-stu-id="2c6e4-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="2c6e4-148">程序</span><span class="sxs-lookup"><span data-stu-id="2c6e4-148">program</span></span>](program.md)               | <span data-ttu-id="2c6e4-149">此控件属于该程序。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="2c6e4-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2c6e4-150">See also</span></span>

| <span data-ttu-id="2c6e4-151">方法</span><span class="sxs-lookup"><span data-stu-id="2c6e4-151">Method</span></span>           | <span data-ttu-id="2c6e4-152">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-152">Return Type</span></span>    |<span data-ttu-id="2c6e4-153">说明</span><span class="sxs-lookup"><span data-stu-id="2c6e4-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c6e4-154">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="2c6e4-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="2c6e4-155">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c6e4-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="2c6e4-156">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="2c6e4-157">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="2c6e4-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="2c6e4-158">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c6e4-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="2c6e4-159">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c6e4-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c6e4-160">JSON representation</span></span>

<span data-ttu-id="2c6e4-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="2c6e4-162">ProgramResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-162">The programResource complex type</span></span>

<span data-ttu-id="2c6e4-163">包含程序 control 对象，该程序资源是引用的对目标的访问审阅的对象的表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="2c6e4-164">此类型继承自`microsoft.graph.identity`，并且具有一个附加属性：</span><span class="sxs-lookup"><span data-stu-id="2c6e4-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="2c6e4-165">属性</span><span class="sxs-lookup"><span data-stu-id="2c6e4-165">Property</span></span>     | <span data-ttu-id="2c6e4-166">类型</span><span class="sxs-lookup"><span data-stu-id="2c6e4-166">Type</span></span>   |<span data-ttu-id="2c6e4-167">说明</span><span class="sxs-lookup"><span data-stu-id="2c6e4-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="2c6e4-168">资源，指明它一组或应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="2c6e4-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
