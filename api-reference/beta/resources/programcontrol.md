---
title: programControl 资源类型
description: 在 Azure AD 访问评审功能中，程序控制对象表示一个控件，将访问评审链接到某个程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 492dc57bfa332472cb7565580ffaa8a5260234c0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443977"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="3da46-103">programControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="3da46-103">programControl resource type</span></span>

<span data-ttu-id="3da46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da46-105">在 Azure AD [访问评审](accessreviews-root.md) 功能中，程序控制对象表示一个控件，将访问评审链接到某个程序。</span><span class="sxs-lookup"><span data-stu-id="3da46-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="3da46-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3da46-106">Methods</span></span>

| <span data-ttu-id="3da46-107">方法</span><span class="sxs-lookup"><span data-stu-id="3da46-107">Method</span></span> | <span data-ttu-id="3da46-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3da46-108">Return Type</span></span> | <span data-ttu-id="3da46-109">说明</span><span class="sxs-lookup"><span data-stu-id="3da46-109">Description</span></span> |
|:------ |:----------- |:----------- |
| [<span data-ttu-id="3da46-110">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="3da46-110">Create programControl</span></span>](../api/programcontrol-create.md) |    [<span data-ttu-id="3da46-111">programControl</span><span class="sxs-lookup"><span data-stu-id="3da46-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="3da46-112">将 programControl 添加到程序。</span><span class="sxs-lookup"><span data-stu-id="3da46-112">Add a programControl to a program.</span></span> |
| [<span data-ttu-id="3da46-113">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="3da46-113">Delete programControl</span></span>](../api/programcontrol-delete.md) | <span data-ttu-id="3da46-114">无。</span><span class="sxs-lookup"><span data-stu-id="3da46-114">None.</span></span> | <span data-ttu-id="3da46-115">从程序中删除 programControl。</span><span class="sxs-lookup"><span data-stu-id="3da46-115">Remove a programControl from a program.</span></span> |
| [<span data-ttu-id="3da46-116">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="3da46-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="3da46-117">[programControl](programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3da46-117">[programControl](programcontrol.md) collection</span></span> | <span data-ttu-id="3da46-118">列出租户中所有程序控件。</span><span class="sxs-lookup"><span data-stu-id="3da46-118">List controls across all programs in the tenant.</span></span> |
| [<span data-ttu-id="3da46-119">列出程序的 programControls</span><span class="sxs-lookup"><span data-stu-id="3da46-119">List programControls of a program</span></span>](../api/program-listcontrols.md) | <span data-ttu-id="3da46-120">[programControl](programcontrol.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3da46-120">[programControl](programcontrol.md) collection</span></span> |    <span data-ttu-id="3da46-121">获取程序控件的集合。</span><span class="sxs-lookup"><span data-stu-id="3da46-121">Get a collection of the controls of a program.</span></span> |
| [<span data-ttu-id="3da46-122">列出 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="3da46-122">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="3da46-123">[programControlType](programcontroltype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3da46-123">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="3da46-124">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="3da46-124">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="3da46-125">属性</span><span class="sxs-lookup"><span data-stu-id="3da46-125">Properties</span></span>

| <span data-ttu-id="3da46-126">属性</span><span class="sxs-lookup"><span data-stu-id="3da46-126">Property</span></span> | <span data-ttu-id="3da46-127">类型</span><span class="sxs-lookup"><span data-stu-id="3da46-127">Type</span></span>   | <span data-ttu-id="3da46-128">说明</span><span class="sxs-lookup"><span data-stu-id="3da46-128">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="3da46-129">id</span><span class="sxs-lookup"><span data-stu-id="3da46-129">id</span></span> | <span data-ttu-id="3da46-130">String</span><span class="sxs-lookup"><span data-stu-id="3da46-130">String</span></span> | <span data-ttu-id="3da46-131">程序与控件之间的链接的功能分配标识符。</span><span class="sxs-lookup"><span data-stu-id="3da46-131">The feature-assigned identifier of the link between program and control.</span></span> |
| <span data-ttu-id="3da46-132">programId</span><span class="sxs-lookup"><span data-stu-id="3da46-132">programId</span></span> | <span data-ttu-id="3da46-133">String</span><span class="sxs-lookup"><span data-stu-id="3da46-133">String</span></span> | <span data-ttu-id="3da46-134">此控件是程序的 programId 的一部分。</span><span class="sxs-lookup"><span data-stu-id="3da46-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="3da46-135">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3da46-135">Required on create.</span></span> |
| <span data-ttu-id="3da46-136">controlId</span><span class="sxs-lookup"><span data-stu-id="3da46-136">controlId</span></span> | <span data-ttu-id="3da46-137">String</span><span class="sxs-lookup"><span data-stu-id="3da46-137">String</span></span> | <span data-ttu-id="3da46-138">控件的 controlId，尤其是访问评审的标识符。</span><span class="sxs-lookup"><span data-stu-id="3da46-138">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="3da46-139">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3da46-139">Required on create.</span></span> |
| <span data-ttu-id="3da46-140">controlTypeId</span><span class="sxs-lookup"><span data-stu-id="3da46-140">controlTypeId</span></span> | <span data-ttu-id="3da46-141">String</span><span class="sxs-lookup"><span data-stu-id="3da46-141">String</span></span> | <span data-ttu-id="3da46-142">programControlType 标识程序控件的类型-例如，链接到来宾访问评审的控件。</span><span class="sxs-lookup"><span data-stu-id="3da46-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="3da46-143">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3da46-143">Required on create.</span></span> |
| <span data-ttu-id="3da46-144">displayName</span><span class="sxs-lookup"><span data-stu-id="3da46-144">displayName</span></span> | <span data-ttu-id="3da46-145">String</span><span class="sxs-lookup"><span data-stu-id="3da46-145">String</span></span> | <span data-ttu-id="3da46-146">控件的名称。</span><span class="sxs-lookup"><span data-stu-id="3da46-146">The name of the control.</span></span> |
| <span data-ttu-id="3da46-147">status</span><span class="sxs-lookup"><span data-stu-id="3da46-147">status</span></span> | <span data-ttu-id="3da46-148">String</span><span class="sxs-lookup"><span data-stu-id="3da46-148">String</span></span> | <span data-ttu-id="3da46-149">控件的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="3da46-149">The life cycle status of the control.</span></span> |
| <span data-ttu-id="3da46-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3da46-150">createdDateTime</span></span> | <span data-ttu-id="3da46-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3da46-151">DateTimeOffset</span></span> | <span data-ttu-id="3da46-152">程序控件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3da46-152">The creation date and time of the program control.</span></span> |
| <span data-ttu-id="3da46-153">所有者</span><span class="sxs-lookup"><span data-stu-id="3da46-153">owner</span></span> | [<span data-ttu-id="3da46-154">userIdentity</span><span class="sxs-lookup"><span data-stu-id="3da46-154">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="3da46-155">创建程序控件的用户。</span><span class="sxs-lookup"><span data-stu-id="3da46-155">The user who created the program control.</span></span> |
| <span data-ttu-id="3da46-156">resource</span><span class="sxs-lookup"><span data-stu-id="3da46-156">resource</span></span> | [<span data-ttu-id="3da46-157">programResource</span><span class="sxs-lookup"><span data-stu-id="3da46-157">programResource</span></span>](programresource.md) | <span data-ttu-id="3da46-158">此程序控件的访问评审针对的资源、组或应用。</span><span class="sxs-lookup"><span data-stu-id="3da46-158">The resource, a group or an app, targeted by this program control's access review.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3da46-159">关系</span><span class="sxs-lookup"><span data-stu-id="3da46-159">Relationships</span></span>

| <span data-ttu-id="3da46-160">关系</span><span class="sxs-lookup"><span data-stu-id="3da46-160">Relationship</span></span> | <span data-ttu-id="3da46-161">类型</span><span class="sxs-lookup"><span data-stu-id="3da46-161">Type</span></span>   | <span data-ttu-id="3da46-162">说明</span><span class="sxs-lookup"><span data-stu-id="3da46-162">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="3da46-163">program</span><span class="sxs-lookup"><span data-stu-id="3da46-163">program</span></span> | [<span data-ttu-id="3da46-164">program</span><span class="sxs-lookup"><span data-stu-id="3da46-164">program</span></span>](program.md) | <span data-ttu-id="3da46-165">此控件属于的程序。</span><span class="sxs-lookup"><span data-stu-id="3da46-165">The program this control is part of.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3da46-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3da46-166">JSON representation</span></span>

<span data-ttu-id="3da46-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3da46-167">Here is a JSON representation of the resource.</span></span>

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


