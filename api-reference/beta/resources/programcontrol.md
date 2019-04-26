---
title: programControl 资源类型
description: 在 Azure AD access 评论功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563333"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="8cc90-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc90-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="8cc90-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="8cc90-105">方法</span><span class="sxs-lookup"><span data-stu-id="8cc90-105">Methods</span></span>

| <span data-ttu-id="8cc90-106">方法</span><span class="sxs-lookup"><span data-stu-id="8cc90-106">Method</span></span>           | <span data-ttu-id="8cc90-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-107">Return Type</span></span>    |<span data-ttu-id="8cc90-108">说明</span><span class="sxs-lookup"><span data-stu-id="8cc90-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cc90-109">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="8cc90-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="8cc90-110">programControl</span><span class="sxs-lookup"><span data-stu-id="8cc90-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="8cc90-111">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="8cc90-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="8cc90-112">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="8cc90-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="8cc90-113">无。</span><span class="sxs-lookup"><span data-stu-id="8cc90-113">None.</span></span>   |   <span data-ttu-id="8cc90-114">从程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="8cc90-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="8cc90-115">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="8cc90-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="8cc90-116">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="8cc90-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8cc90-117">列出租户中所有程序之间的控件。</span><span class="sxs-lookup"><span data-stu-id="8cc90-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="8cc90-118">权限</span><span class="sxs-lookup"><span data-stu-id="8cc90-118">Permissions</span></span>

|<span data-ttu-id="8cc90-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-119">Permission type</span></span>                        | <span data-ttu-id="8cc90-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cc90-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc90-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cc90-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cc90-122">ProgramControl、ProgramControl 和所有</span><span class="sxs-lookup"><span data-stu-id="8cc90-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="8cc90-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cc90-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc90-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cc90-124">Not supported.</span></span> |
|<span data-ttu-id="8cc90-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cc90-125">Application</span></span>                            | <span data-ttu-id="8cc90-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cc90-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="8cc90-127">属性</span><span class="sxs-lookup"><span data-stu-id="8cc90-127">Properties</span></span>
| <span data-ttu-id="8cc90-128">属性</span><span class="sxs-lookup"><span data-stu-id="8cc90-128">Property</span></span>     | <span data-ttu-id="8cc90-129">类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-129">Type</span></span>   |<span data-ttu-id="8cc90-130">说明</span><span class="sxs-lookup"><span data-stu-id="8cc90-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="8cc90-131">程序和控件之间的链接的功能分配的标识符</span><span class="sxs-lookup"><span data-stu-id="8cc90-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="8cc90-132">此控件所属程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="8cc90-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="8cc90-133">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="8cc90-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="8cc90-134">控件的 controlId, 特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="8cc90-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="8cc90-135">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="8cc90-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="8cc90-136">programControlType 标识程序控制的类型-例如, 链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="8cc90-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="8cc90-137">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="8cc90-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="8cc90-138">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="8cc90-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="8cc90-139">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="8cc90-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="8cc90-140">程序控件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8cc90-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="8cc90-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="8cc90-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="8cc90-142">创建程序控件的用户。</span><span class="sxs-lookup"><span data-stu-id="8cc90-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="8cc90-143">由该程序控件的访问审核作为目标的资源、组或应用程序。</span><span class="sxs-lookup"><span data-stu-id="8cc90-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="8cc90-144">关系</span><span class="sxs-lookup"><span data-stu-id="8cc90-144">Relationships</span></span>
| <span data-ttu-id="8cc90-145">关系</span><span class="sxs-lookup"><span data-stu-id="8cc90-145">Relationship</span></span> | <span data-ttu-id="8cc90-146">类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-146">Type</span></span>   |<span data-ttu-id="8cc90-147">说明</span><span class="sxs-lookup"><span data-stu-id="8cc90-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="8cc90-148">主程序</span><span class="sxs-lookup"><span data-stu-id="8cc90-148">program</span></span>](program.md)               | <span data-ttu-id="8cc90-149">此控件所属的程序。</span><span class="sxs-lookup"><span data-stu-id="8cc90-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="8cc90-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8cc90-150">See also</span></span>

| <span data-ttu-id="8cc90-151">方法</span><span class="sxs-lookup"><span data-stu-id="8cc90-151">Method</span></span>           | <span data-ttu-id="8cc90-152">返回类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-152">Return Type</span></span>    |<span data-ttu-id="8cc90-153">说明</span><span class="sxs-lookup"><span data-stu-id="8cc90-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cc90-154">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="8cc90-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="8cc90-155">[programControl](programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="8cc90-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8cc90-156">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="8cc90-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8cc90-157">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="8cc90-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="8cc90-158">[programControlType](programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="8cc90-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="8cc90-159">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="8cc90-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8cc90-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cc90-160">JSON representation</span></span>

<span data-ttu-id="8cc90-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cc90-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="8cc90-162">programResource 复杂类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-162">The programResource complex type</span></span>

<span data-ttu-id="8cc90-163">程序控制对象中包含的程序资源是对作为访问评审目标的对象的引用的表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cc90-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="8cc90-164">此类型将从`microsoft.graph.identity`继承并包含一个附加属性:</span><span class="sxs-lookup"><span data-stu-id="8cc90-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="8cc90-165">属性</span><span class="sxs-lookup"><span data-stu-id="8cc90-165">Property</span></span>     | <span data-ttu-id="8cc90-166">类型</span><span class="sxs-lookup"><span data-stu-id="8cc90-166">Type</span></span>   |<span data-ttu-id="8cc90-167">说明</span><span class="sxs-lookup"><span data-stu-id="8cc90-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="8cc90-168">资源的类型, 指示它是一个组还是一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="8cc90-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
