---
title: programControl 资源类型
description: 在 Azure AD access 评论功能中，program control 对象表示一个控件，将访问权限链接到某个程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 9837f160015dedb0f37cce65b8209ff9a6ec5331
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330163"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="f5f46-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5f46-103">programControl resource type</span></span>

<span data-ttu-id="f5f46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5f46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f46-105">在 Azure AD [access 评论](accessreviews-root.md) 功能中，program control 对象表示一个控件，将访问权限链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="f5f46-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="f5f46-106">方法</span><span class="sxs-lookup"><span data-stu-id="f5f46-106">Methods</span></span>

| <span data-ttu-id="f5f46-107">方法</span><span class="sxs-lookup"><span data-stu-id="f5f46-107">Method</span></span> | <span data-ttu-id="f5f46-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5f46-108">Return Type</span></span> | <span data-ttu-id="f5f46-109">说明</span><span class="sxs-lookup"><span data-stu-id="f5f46-109">Description</span></span> |
|:------ |:----------- |:----------- |
| [<span data-ttu-id="f5f46-110">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="f5f46-110">Create programControl</span></span>](../api/programcontrol-create.md) |    [<span data-ttu-id="f5f46-111">programControl</span><span class="sxs-lookup"><span data-stu-id="f5f46-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="f5f46-112">将 programControl 添加到程序中。</span><span class="sxs-lookup"><span data-stu-id="f5f46-112">Add a programControl to a program.</span></span> |
| [<span data-ttu-id="f5f46-113">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="f5f46-113">Delete programControl</span></span>](../api/programcontrol-delete.md) | <span data-ttu-id="f5f46-114">无。</span><span class="sxs-lookup"><span data-stu-id="f5f46-114">None.</span></span> | <span data-ttu-id="f5f46-115">从程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="f5f46-115">Remove a programControl from a program.</span></span> |
| [<span data-ttu-id="f5f46-116">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="f5f46-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="f5f46-117">[programControl](programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5f46-117">[programControl](programcontrol.md) collection</span></span> | <span data-ttu-id="f5f46-118">列出租户中所有程序之间的控件。</span><span class="sxs-lookup"><span data-stu-id="f5f46-118">List controls across all programs in the tenant.</span></span> |
| [<span data-ttu-id="f5f46-119">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="f5f46-119">List programControls of a program</span></span>](../api/program-listcontrols.md) | <span data-ttu-id="f5f46-120">[programControl](programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5f46-120">[programControl](programcontrol.md) collection</span></span> |    <span data-ttu-id="f5f46-121">获取程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="f5f46-121">Get a collection of the controls of a program.</span></span> |
| [<span data-ttu-id="f5f46-122">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f5f46-122">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="f5f46-123">[programControlType](programcontroltype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5f46-123">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="f5f46-124">列出程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="f5f46-124">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="f5f46-125">属性</span><span class="sxs-lookup"><span data-stu-id="f5f46-125">Properties</span></span>

| <span data-ttu-id="f5f46-126">属性</span><span class="sxs-lookup"><span data-stu-id="f5f46-126">Property</span></span> | <span data-ttu-id="f5f46-127">类型</span><span class="sxs-lookup"><span data-stu-id="f5f46-127">Type</span></span>   | <span data-ttu-id="f5f46-128">说明</span><span class="sxs-lookup"><span data-stu-id="f5f46-128">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="f5f46-129">id</span><span class="sxs-lookup"><span data-stu-id="f5f46-129">id</span></span> | <span data-ttu-id="f5f46-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f5f46-130">String</span></span> | <span data-ttu-id="f5f46-131">程序和控件之间的链接的功能分配的标识符。</span><span class="sxs-lookup"><span data-stu-id="f5f46-131">The feature-assigned identifier of the link between program and control.</span></span> |
| <span data-ttu-id="f5f46-132">programId</span><span class="sxs-lookup"><span data-stu-id="f5f46-132">programId</span></span> | <span data-ttu-id="f5f46-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f5f46-133">String</span></span> | <span data-ttu-id="f5f46-134">此控件所属程序的 programId。</span><span class="sxs-lookup"><span data-stu-id="f5f46-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="f5f46-135">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="f5f46-135">Required on create.</span></span> |
| <span data-ttu-id="f5f46-136">controlId</span><span class="sxs-lookup"><span data-stu-id="f5f46-136">controlId</span></span> | <span data-ttu-id="f5f46-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f5f46-137">String</span></span> | <span data-ttu-id="f5f46-138">控件的 controlId，特别是 access 评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="f5f46-138">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="f5f46-139">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="f5f46-139">Required on create.</span></span> |
| <span data-ttu-id="f5f46-140">controlTypeId</span><span class="sxs-lookup"><span data-stu-id="f5f46-140">controlTypeId</span></span> | <span data-ttu-id="f5f46-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f5f46-141">String</span></span> | <span data-ttu-id="f5f46-142">ProgramControlType 标识程序控制的类型-例如，链接到来宾访问审阅的控件。</span><span class="sxs-lookup"><span data-stu-id="f5f46-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="f5f46-143">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="f5f46-143">Required on create.</span></span> |
| <span data-ttu-id="f5f46-144">displayName</span><span class="sxs-lookup"><span data-stu-id="f5f46-144">displayName</span></span> | <span data-ttu-id="f5f46-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f5f46-145">String</span></span> | <span data-ttu-id="f5f46-146">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="f5f46-146">The name of the control.</span></span> |
| <span data-ttu-id="f5f46-147">状态</span><span class="sxs-lookup"><span data-stu-id="f5f46-147">status</span></span> | <span data-ttu-id="f5f46-148">字符串</span><span class="sxs-lookup"><span data-stu-id="f5f46-148">String</span></span> | <span data-ttu-id="f5f46-149">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="f5f46-149">The life cycle status of the control.</span></span> |
| <span data-ttu-id="f5f46-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5f46-150">createdDateTime</span></span> | <span data-ttu-id="f5f46-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5f46-151">DateTimeOffset</span></span> | <span data-ttu-id="f5f46-152">程序控件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f5f46-152">The creation date and time of the program control.</span></span> |
| <span data-ttu-id="f5f46-153">owner</span><span class="sxs-lookup"><span data-stu-id="f5f46-153">owner</span></span> | [<span data-ttu-id="f5f46-154">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f5f46-154">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="f5f46-155">创建程序控件的用户。</span><span class="sxs-lookup"><span data-stu-id="f5f46-155">The user who created the program control.</span></span> |
| <span data-ttu-id="f5f46-156">resource</span><span class="sxs-lookup"><span data-stu-id="f5f46-156">resource</span></span> | [<span data-ttu-id="f5f46-157">programResource</span><span class="sxs-lookup"><span data-stu-id="f5f46-157">programResource</span></span>](programresource.md) | <span data-ttu-id="f5f46-158">由该程序控件的访问审核作为目标的资源、组或应用程序。</span><span class="sxs-lookup"><span data-stu-id="f5f46-158">The resource, a group or an app, targeted by this program control's access review.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f5f46-159">关系</span><span class="sxs-lookup"><span data-stu-id="f5f46-159">Relationships</span></span>

| <span data-ttu-id="f5f46-160">关系</span><span class="sxs-lookup"><span data-stu-id="f5f46-160">Relationship</span></span> | <span data-ttu-id="f5f46-161">类型</span><span class="sxs-lookup"><span data-stu-id="f5f46-161">Type</span></span>   | <span data-ttu-id="f5f46-162">说明</span><span class="sxs-lookup"><span data-stu-id="f5f46-162">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="f5f46-163">主程序</span><span class="sxs-lookup"><span data-stu-id="f5f46-163">program</span></span> | [<span data-ttu-id="f5f46-164">主程序</span><span class="sxs-lookup"><span data-stu-id="f5f46-164">program</span></span>](program.md) | <span data-ttu-id="f5f46-165">此控件所属的程序。</span><span class="sxs-lookup"><span data-stu-id="f5f46-165">The program this control is part of.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f5f46-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5f46-166">JSON representation</span></span>

<span data-ttu-id="f5f46-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5f46-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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


