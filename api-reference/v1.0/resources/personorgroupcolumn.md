---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: columnDefinition 资源上的 personOrGroupColumn 指示列值，该值表示从目录中选择的个人或组。
doc_type: resourcePageType
ms.openlocfilehash: d8ce31e7eb044e588f73afefb2b370e161fa7cdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035516"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="c666a-103">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c666a-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="c666a-104">[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="c666a-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c666a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c666a-105">JSON representation</span></span>

<span data-ttu-id="c666a-106">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c666a-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="c666a-107">属性</span><span class="sxs-lookup"><span data-stu-id="c666a-107">Properties</span></span>

| <span data-ttu-id="c666a-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="c666a-108">Property name</span></span>              | <span data-ttu-id="c666a-109">类型</span><span class="sxs-lookup"><span data-stu-id="c666a-109">Type</span></span>    | <span data-ttu-id="c666a-110">说明</span><span class="sxs-lookup"><span data-stu-id="c666a-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="c666a-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="c666a-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="c666a-112">boolean</span><span class="sxs-lookup"><span data-stu-id="c666a-112">boolean</span></span> | <span data-ttu-id="c666a-113">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="c666a-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="c666a-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="c666a-114">**displayAs**</span></span>              | <span data-ttu-id="c666a-115">string</span><span class="sxs-lookup"><span data-stu-id="c666a-115">string</span></span>  | <span data-ttu-id="c666a-116">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="c666a-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="c666a-117">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="c666a-117">See below.</span></span>
| <span data-ttu-id="c666a-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="c666a-118">**chooseFromType**</span></span>         | <span data-ttu-id="c666a-119">string</span><span class="sxs-lookup"><span data-stu-id="c666a-119">string</span></span>  | <span data-ttu-id="c666a-120">是否允许仅选择人员，或同时选择人员和组。</span><span class="sxs-lookup"><span data-stu-id="c666a-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="c666a-121">必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="c666a-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="c666a-122">DisplayAs 选项</span><span class="sxs-lookup"><span data-stu-id="c666a-122">DisplayAs options</span></span>

| <span data-ttu-id="c666a-123">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="c666a-123">DisplayAs value</span></span>               | <span data-ttu-id="c666a-124">说明</span><span class="sxs-lookup"><span data-stu-id="c666a-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="c666a-125">**帐户**</span><span class="sxs-lookup"><span data-stu-id="c666a-125">**account**</span></span>                   | <span data-ttu-id="c666a-126">采用原始 SharePoint 编码的人员或组声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="c666a-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="c666a-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="c666a-127">i:0#.f</span></span>|<span data-ttu-id="c666a-128">membership</span><span class="sxs-lookup"><span data-stu-id="c666a-128">membership</span></span>|<span data-ttu-id="c666a-129">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="c666a-129">jane@contoso.com).</span></span>
| <span data-ttu-id="c666a-130">**department**</span><span class="sxs-lookup"><span data-stu-id="c666a-130">**department**</span></span>                | <span data-ttu-id="c666a-131">人员或组的所在部门。</span><span class="sxs-lookup"><span data-stu-id="c666a-131">The person or group's department.</span></span>
| <span data-ttu-id="c666a-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="c666a-132">**firstName**</span></span>                 | <span data-ttu-id="c666a-133">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="c666a-133">The person's first name.</span></span>
| <span data-ttu-id="c666a-134">**id**</span><span class="sxs-lookup"><span data-stu-id="c666a-134">**id**</span></span>                        | <span data-ttu-id="c666a-135">目录中个人或组的 id。</span><span class="sxs-lookup"><span data-stu-id="c666a-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="c666a-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="c666a-136">**lastName**</span></span>                  | <span data-ttu-id="c666a-137">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="c666a-137">The person's last name.</span></span>
| <span data-ttu-id="c666a-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="c666a-138">**mobilePhone**</span></span>               | <span data-ttu-id="c666a-139">人员的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="c666a-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="c666a-140">**name**</span><span class="sxs-lookup"><span data-stu-id="c666a-140">**name**</span></span>                      | <span data-ttu-id="c666a-141">人员姓名。</span><span class="sxs-lookup"><span data-stu-id="c666a-141">The person's name.</span></span>
| <span data-ttu-id="c666a-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="c666a-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="c666a-143">人员姓名，以及他们的照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="c666a-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="c666a-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="c666a-144">**nameWithPresence**</span></span>          | <span data-ttu-id="c666a-145">默认值。</span><span class="sxs-lookup"><span data-stu-id="c666a-145">Default.</span></span> <span data-ttu-id="c666a-146">人员姓名和状态指示器图标（空闲/忙碌/等）</span><span class="sxs-lookup"><span data-stu-id="c666a-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="c666a-147">**office**</span><span class="sxs-lookup"><span data-stu-id="c666a-147">**office**</span></span>                    | <span data-ttu-id="c666a-148">人员的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="c666a-148">The person's office number.</span></span>
| <span data-ttu-id="c666a-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="c666a-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="c666a-150">人员的照片，采用 36x36 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="c666a-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="c666a-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="c666a-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="c666a-152">人员的照片，采用 48x48 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="c666a-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="c666a-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="c666a-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="c666a-154">人员的照片，采用 72x72 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="c666a-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="c666a-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="c666a-155">**sipAddress**</span></span>                | <span data-ttu-id="c666a-156">人员的 sip 地址。</span><span class="sxs-lookup"><span data-stu-id="c666a-156">The person's sip address.</span></span>
| <span data-ttu-id="c666a-157">**title**</span><span class="sxs-lookup"><span data-stu-id="c666a-157">**title**</span></span>                     | <span data-ttu-id="c666a-158">人员在组织中的职务。</span><span class="sxs-lookup"><span data-stu-id="c666a-158">The person's title in the organization.</span></span>
| <span data-ttu-id="c666a-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="c666a-159">**userName**</span></span>                  | <span data-ttu-id="c666a-160">人员或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="c666a-160">The person or group's user name.</span></span>
| <span data-ttu-id="c666a-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="c666a-161">**workEmail**</span></span>                 | <span data-ttu-id="c666a-162">人员或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c666a-162">The person or group's email address.</span></span>
| <span data-ttu-id="c666a-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="c666a-163">**workPhone**</span></span>                 | <span data-ttu-id="c666a-164">人员的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="c666a-164">The person's work phone number.</span></span>

<span data-ttu-id="c666a-165">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="c666a-165">Note: Additional DisplayAs types may be returned.</span></span>

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
