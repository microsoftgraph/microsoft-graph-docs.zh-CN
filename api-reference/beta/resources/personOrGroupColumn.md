---
author: simonhult
description: columnDefinition 资源上的 personOrGroupColumn 指示列值，该值表示从目录中选择的个人或组。
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 24daf2ffd48e7647c898031aee634e8a84e05ee0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966151"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="c1db1-103">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1db1-103">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1db1-104">[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="c1db1-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1db1-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1db1-105">JSON representation</span></span>

<span data-ttu-id="c1db1-106">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1db1-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="c1db1-107">属性</span><span class="sxs-lookup"><span data-stu-id="c1db1-107">Properties</span></span>

| <span data-ttu-id="c1db1-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="c1db1-108">Property name</span></span>              | <span data-ttu-id="c1db1-109">类型</span><span class="sxs-lookup"><span data-stu-id="c1db1-109">Type</span></span>    | <span data-ttu-id="c1db1-110">说明</span><span class="sxs-lookup"><span data-stu-id="c1db1-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="c1db1-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="c1db1-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="c1db1-112">boolean</span><span class="sxs-lookup"><span data-stu-id="c1db1-112">boolean</span></span> | <span data-ttu-id="c1db1-113">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="c1db1-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="c1db1-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="c1db1-114">**displayAs**</span></span>              | <span data-ttu-id="c1db1-115">string</span><span class="sxs-lookup"><span data-stu-id="c1db1-115">string</span></span>  | <span data-ttu-id="c1db1-116">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="c1db1-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="c1db1-117">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="c1db1-117">See below.</span></span>
| <span data-ttu-id="c1db1-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="c1db1-118">**chooseFromType**</span></span>         | <span data-ttu-id="c1db1-119">string</span><span class="sxs-lookup"><span data-stu-id="c1db1-119">string</span></span>  | <span data-ttu-id="c1db1-120">是否允许仅选择人员，或同时选择人员和组。</span><span class="sxs-lookup"><span data-stu-id="c1db1-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="c1db1-121">必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="c1db1-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="c1db1-122">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="c1db1-122">DisplayAs values</span></span>

| <span data-ttu-id="c1db1-123">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="c1db1-123">DisplayAs value</span></span>               | <span data-ttu-id="c1db1-124">说明</span><span class="sxs-lookup"><span data-stu-id="c1db1-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="c1db1-125">**帐户**</span><span class="sxs-lookup"><span data-stu-id="c1db1-125">**account**</span></span>                   | <span data-ttu-id="c1db1-126">采用原始 SharePoint 编码的人员或组声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="c1db1-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="c1db1-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="c1db1-127">i:0#.f</span></span>|<span data-ttu-id="c1db1-128">membership</span><span class="sxs-lookup"><span data-stu-id="c1db1-128">membership</span></span>|<span data-ttu-id="c1db1-129">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="c1db1-129">jane@contoso.com).</span></span>
| <span data-ttu-id="c1db1-130">**department**</span><span class="sxs-lookup"><span data-stu-id="c1db1-130">**department**</span></span>                | <span data-ttu-id="c1db1-131">人员或组的所在部门。</span><span class="sxs-lookup"><span data-stu-id="c1db1-131">The person or group's department.</span></span>
| <span data-ttu-id="c1db1-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="c1db1-132">**firstName**</span></span>                 | <span data-ttu-id="c1db1-133">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="c1db1-133">The person's first name.</span></span>
| <span data-ttu-id="c1db1-134">**id**</span><span class="sxs-lookup"><span data-stu-id="c1db1-134">**id**</span></span>                        | <span data-ttu-id="c1db1-135">目录中个人或组的 id。</span><span class="sxs-lookup"><span data-stu-id="c1db1-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="c1db1-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="c1db1-136">**lastName**</span></span>                  | <span data-ttu-id="c1db1-137">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="c1db1-137">The person's last name.</span></span>
| <span data-ttu-id="c1db1-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="c1db1-138">**mobilePhone**</span></span>               | <span data-ttu-id="c1db1-139">人员的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="c1db1-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="c1db1-140">**name**</span><span class="sxs-lookup"><span data-stu-id="c1db1-140">**name**</span></span>                      | <span data-ttu-id="c1db1-141">人员姓名。</span><span class="sxs-lookup"><span data-stu-id="c1db1-141">The person's name.</span></span>
| <span data-ttu-id="c1db1-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="c1db1-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="c1db1-143">人员姓名，以及他们的照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="c1db1-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="c1db1-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="c1db1-144">**nameWithPresence**</span></span>          | <span data-ttu-id="c1db1-145">默认值。</span><span class="sxs-lookup"><span data-stu-id="c1db1-145">Default.</span></span> <span data-ttu-id="c1db1-146">人员姓名和状态指示器图标（空闲/忙碌/等）</span><span class="sxs-lookup"><span data-stu-id="c1db1-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="c1db1-147">**office**</span><span class="sxs-lookup"><span data-stu-id="c1db1-147">**office**</span></span>                    | <span data-ttu-id="c1db1-148">人员的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="c1db1-148">The person's office number.</span></span>
| <span data-ttu-id="c1db1-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="c1db1-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="c1db1-150">人员的照片，采用 36x36 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="c1db1-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="c1db1-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="c1db1-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="c1db1-152">人员的照片，采用 48x48 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="c1db1-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="c1db1-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="c1db1-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="c1db1-154">人员的照片，采用 72x72 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="c1db1-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="c1db1-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="c1db1-155">**sipAddress**</span></span>                | <span data-ttu-id="c1db1-156">人员的 sip 地址。</span><span class="sxs-lookup"><span data-stu-id="c1db1-156">The person's sip address.</span></span>
| <span data-ttu-id="c1db1-157">**title**</span><span class="sxs-lookup"><span data-stu-id="c1db1-157">**title**</span></span>                     | <span data-ttu-id="c1db1-158">人员在组织中的职务。</span><span class="sxs-lookup"><span data-stu-id="c1db1-158">The person's title in the organization.</span></span>
| <span data-ttu-id="c1db1-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="c1db1-159">**userName**</span></span>                  | <span data-ttu-id="c1db1-160">人员或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="c1db1-160">The person or group's user name.</span></span>
| <span data-ttu-id="c1db1-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="c1db1-161">**workEmail**</span></span>                 | <span data-ttu-id="c1db1-162">人员或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c1db1-162">The person or group's email address.</span></span>
| <span data-ttu-id="c1db1-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="c1db1-163">**workPhone**</span></span>                 | <span data-ttu-id="c1db1-164">人员的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="c1db1-164">The person's work phone number.</span></span>

<span data-ttu-id="c1db1-165">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="c1db1-165">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": []
}
-->
