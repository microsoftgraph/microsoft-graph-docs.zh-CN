---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a1eb5b36f2af7b66da7fd891ccd324fa325504c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923465"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="99a86-102">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="99a86-102">PersonOrGroupColumn resource type</span></span>

> <span data-ttu-id="99a86-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99a86-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99a86-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99a86-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99a86-105">[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="99a86-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99a86-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99a86-106">JSON representation</span></span>

<span data-ttu-id="99a86-107">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99a86-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="99a86-108">属性</span><span class="sxs-lookup"><span data-stu-id="99a86-108">Properties</span></span>

| <span data-ttu-id="99a86-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="99a86-109">Property name</span></span>              | <span data-ttu-id="99a86-110">类型</span><span class="sxs-lookup"><span data-stu-id="99a86-110">Type</span></span>    | <span data-ttu-id="99a86-111">说明</span><span class="sxs-lookup"><span data-stu-id="99a86-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="99a86-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="99a86-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="99a86-113">boolean</span><span class="sxs-lookup"><span data-stu-id="99a86-113">boolean</span></span> | <span data-ttu-id="99a86-114">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="99a86-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="99a86-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="99a86-115">**displayAs**</span></span>              | <span data-ttu-id="99a86-116">string</span><span class="sxs-lookup"><span data-stu-id="99a86-116">string</span></span>  | <span data-ttu-id="99a86-117">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="99a86-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="99a86-118">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="99a86-118">See below.</span></span>
| <span data-ttu-id="99a86-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="99a86-119">**chooseFromType**</span></span>         | <span data-ttu-id="99a86-120">string</span><span class="sxs-lookup"><span data-stu-id="99a86-120">string</span></span>  | <span data-ttu-id="99a86-121">是否允许仅选择人员，或同时选择人员和组。</span><span class="sxs-lookup"><span data-stu-id="99a86-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="99a86-122">必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="99a86-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="99a86-123">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="99a86-123">DisplayAs values</span></span>

| <span data-ttu-id="99a86-124">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="99a86-124">DisplayAs value</span></span>               | <span data-ttu-id="99a86-125">说明</span><span class="sxs-lookup"><span data-stu-id="99a86-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="99a86-126">**帐户**</span><span class="sxs-lookup"><span data-stu-id="99a86-126">**account**</span></span>                   | <span data-ttu-id="99a86-127">采用原始 SharePoint 编码的人员或组声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="99a86-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="99a86-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="99a86-128">i:0#.f</span></span>|<span data-ttu-id="99a86-129">membership</span><span class="sxs-lookup"><span data-stu-id="99a86-129">membership</span></span>|<span data-ttu-id="99a86-130">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="99a86-130">jane@contoso.com).</span></span>
| <span data-ttu-id="99a86-131">**department**</span><span class="sxs-lookup"><span data-stu-id="99a86-131">**department**</span></span>                | <span data-ttu-id="99a86-132">人员或组的所在部门。</span><span class="sxs-lookup"><span data-stu-id="99a86-132">The person or group's department.</span></span>
| <span data-ttu-id="99a86-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="99a86-133">**firstName**</span></span>                 | <span data-ttu-id="99a86-134">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="99a86-134">The person's first name.</span></span>
| <span data-ttu-id="99a86-135">**id**</span><span class="sxs-lookup"><span data-stu-id="99a86-135">**id**</span></span>                        | <span data-ttu-id="99a86-136">目录中个人或组的 id。</span><span class="sxs-lookup"><span data-stu-id="99a86-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="99a86-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="99a86-137">**lastName**</span></span>                  | <span data-ttu-id="99a86-138">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="99a86-138">The person's last name.</span></span>
| <span data-ttu-id="99a86-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="99a86-139">**mobilePhone**</span></span>               | <span data-ttu-id="99a86-140">人员的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="99a86-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="99a86-141">**name**</span><span class="sxs-lookup"><span data-stu-id="99a86-141">**name**</span></span>                      | <span data-ttu-id="99a86-142">人员姓名。</span><span class="sxs-lookup"><span data-stu-id="99a86-142">The person's name.</span></span>
| <span data-ttu-id="99a86-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="99a86-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="99a86-144">人员姓名，以及他们的照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="99a86-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="99a86-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="99a86-145">**nameWithPresence**</span></span>          | <span data-ttu-id="99a86-146">默认值。</span><span class="sxs-lookup"><span data-stu-id="99a86-146">Default.</span></span> <span data-ttu-id="99a86-147">人员姓名和状态指示器图标（空闲/忙碌/等）</span><span class="sxs-lookup"><span data-stu-id="99a86-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="99a86-148">**office**</span><span class="sxs-lookup"><span data-stu-id="99a86-148">**office**</span></span>                    | <span data-ttu-id="99a86-149">人员的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="99a86-149">The person's office number.</span></span>
| <span data-ttu-id="99a86-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="99a86-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="99a86-151">人员的照片，采用 36x36 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="99a86-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="99a86-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="99a86-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="99a86-153">人员的照片，采用 48x48 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="99a86-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="99a86-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="99a86-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="99a86-155">人员的照片，采用 72x72 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="99a86-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="99a86-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="99a86-156">**sipAddress**</span></span>                | <span data-ttu-id="99a86-157">人员的 sip 地址。</span><span class="sxs-lookup"><span data-stu-id="99a86-157">The person's sip address.</span></span>
| <span data-ttu-id="99a86-158">**title**</span><span class="sxs-lookup"><span data-stu-id="99a86-158">**title**</span></span>                     | <span data-ttu-id="99a86-159">人员在组织中的职务。</span><span class="sxs-lookup"><span data-stu-id="99a86-159">The person's title in the organization.</span></span>
| <span data-ttu-id="99a86-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="99a86-160">**userName**</span></span>                  | <span data-ttu-id="99a86-161">人员或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="99a86-161">The person or group's user name.</span></span>
| <span data-ttu-id="99a86-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="99a86-162">**workEmail**</span></span>                 | <span data-ttu-id="99a86-163">人员或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="99a86-163">The person or group's email address.</span></span>
| <span data-ttu-id="99a86-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="99a86-164">**workPhone**</span></span>                 | <span data-ttu-id="99a86-165">人员的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="99a86-165">The person's work phone number.</span></span>

<span data-ttu-id="99a86-166">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="99a86-166">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
