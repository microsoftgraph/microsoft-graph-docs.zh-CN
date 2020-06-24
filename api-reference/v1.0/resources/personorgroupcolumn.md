---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: columnDefinition 资源上的 personOrGroupColumn 指示列值，该值表示从目录中选择的个人或组。
doc_type: resourcePageType
ms.openlocfilehash: b9c3774405dbb8d2e98a9823a84be97d5df09b0b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845475"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="a119e-103">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="a119e-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="a119e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a119e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a119e-105">[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="a119e-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a119e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a119e-106">JSON representation</span></span>

<span data-ttu-id="a119e-107">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a119e-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="a119e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a119e-108">Properties</span></span>

| <span data-ttu-id="a119e-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="a119e-109">Property name</span></span>              | <span data-ttu-id="a119e-110">类型</span><span class="sxs-lookup"><span data-stu-id="a119e-110">Type</span></span>    | <span data-ttu-id="a119e-111">Description</span><span class="sxs-lookup"><span data-stu-id="a119e-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="a119e-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="a119e-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="a119e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="a119e-113">boolean</span></span> | <span data-ttu-id="a119e-114">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="a119e-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a119e-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a119e-115">**displayAs**</span></span>              | <span data-ttu-id="a119e-116">字符串</span><span class="sxs-lookup"><span data-stu-id="a119e-116">string</span></span>  | <span data-ttu-id="a119e-117">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="a119e-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="a119e-118">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="a119e-118">See below.</span></span>
| <span data-ttu-id="a119e-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="a119e-119">**chooseFromType**</span></span>         | <span data-ttu-id="a119e-120">string</span><span class="sxs-lookup"><span data-stu-id="a119e-120">string</span></span>  | <span data-ttu-id="a119e-121">是否允许仅选择人员，或同时选择人员和组。</span><span class="sxs-lookup"><span data-stu-id="a119e-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="a119e-122">必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="a119e-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="a119e-123">DisplayAs 选项</span><span class="sxs-lookup"><span data-stu-id="a119e-123">DisplayAs options</span></span>

| <span data-ttu-id="a119e-124">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="a119e-124">DisplayAs value</span></span>               | <span data-ttu-id="a119e-125">说明</span><span class="sxs-lookup"><span data-stu-id="a119e-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="a119e-126">**帐户**</span><span class="sxs-lookup"><span data-stu-id="a119e-126">**account**</span></span>                   | <span data-ttu-id="a119e-127">采用原始 SharePoint 编码的人员或组声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="a119e-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="a119e-128">`i:0#.f|membership|jane@contoso.com`).</span><span class="sxs-lookup"><span data-stu-id="a119e-128">`i:0#.f|membership|jane@contoso.com`).</span></span>
| <span data-ttu-id="a119e-129">**department**</span><span class="sxs-lookup"><span data-stu-id="a119e-129">**department**</span></span>                | <span data-ttu-id="a119e-130">人员或组的所在部门。</span><span class="sxs-lookup"><span data-stu-id="a119e-130">The person or group's department.</span></span>
| <span data-ttu-id="a119e-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="a119e-131">**firstName**</span></span>                 | <span data-ttu-id="a119e-132">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="a119e-132">The person's first name.</span></span>
| <span data-ttu-id="a119e-133">**id**</span><span class="sxs-lookup"><span data-stu-id="a119e-133">**id**</span></span>                        | <span data-ttu-id="a119e-134">目录中个人或组的 id。</span><span class="sxs-lookup"><span data-stu-id="a119e-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="a119e-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="a119e-135">**lastName**</span></span>                  | <span data-ttu-id="a119e-136">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="a119e-136">The person's last name.</span></span>
| <span data-ttu-id="a119e-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="a119e-137">**mobilePhone**</span></span>               | <span data-ttu-id="a119e-138">人员的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="a119e-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="a119e-139">**name**</span><span class="sxs-lookup"><span data-stu-id="a119e-139">**name**</span></span>                      | <span data-ttu-id="a119e-140">人员姓名。</span><span class="sxs-lookup"><span data-stu-id="a119e-140">The person's name.</span></span>
| <span data-ttu-id="a119e-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="a119e-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="a119e-142">人员姓名，以及他们的照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a119e-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="a119e-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="a119e-143">**nameWithPresence**</span></span>          | <span data-ttu-id="a119e-144">默认值。</span><span class="sxs-lookup"><span data-stu-id="a119e-144">Default.</span></span> <span data-ttu-id="a119e-145">人员姓名和状态指示器图标（空闲/忙碌/等）</span><span class="sxs-lookup"><span data-stu-id="a119e-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="a119e-146">**office**</span><span class="sxs-lookup"><span data-stu-id="a119e-146">**office**</span></span>                    | <span data-ttu-id="a119e-147">人员的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="a119e-147">The person's office number.</span></span>
| <span data-ttu-id="a119e-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="a119e-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="a119e-149">人员的照片，采用 36x36 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="a119e-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="a119e-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="a119e-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="a119e-151">人员的照片，采用 48x48 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="a119e-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="a119e-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="a119e-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="a119e-153">人员的照片，采用 72x72 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="a119e-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="a119e-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="a119e-154">**sipAddress**</span></span>                | <span data-ttu-id="a119e-155">人员的 sip 地址。</span><span class="sxs-lookup"><span data-stu-id="a119e-155">The person's sip address.</span></span>
| <span data-ttu-id="a119e-156">**title**</span><span class="sxs-lookup"><span data-stu-id="a119e-156">**title**</span></span>                     | <span data-ttu-id="a119e-157">人员在组织中的职务。</span><span class="sxs-lookup"><span data-stu-id="a119e-157">The person's title in the organization.</span></span>
| <span data-ttu-id="a119e-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="a119e-158">**userName**</span></span>                  | <span data-ttu-id="a119e-159">人员或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="a119e-159">The person or group's user name.</span></span>
| <span data-ttu-id="a119e-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="a119e-160">**workEmail**</span></span>                 | <span data-ttu-id="a119e-161">人员或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a119e-161">The person or group's email address.</span></span>
| <span data-ttu-id="a119e-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="a119e-162">**workPhone**</span></span>                 | <span data-ttu-id="a119e-163">人员的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="a119e-163">The person's work phone number.</span></span>

<span data-ttu-id="a119e-164">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="a119e-164">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
