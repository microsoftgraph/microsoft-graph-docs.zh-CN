---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 715c6ca22957cbd951784e6cf32edf2bf47f1098
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="d19cd-102">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="d19cd-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="d19cd-103">[columnDefinition](columnDefinition.md) 资源上的 **personOrGroupColumn** 指示列值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="d19cd-103">The **personOrGroupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d19cd-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d19cd-104">JSON representation</span></span>

<span data-ttu-id="d19cd-105">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d19cd-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="d19cd-106">属性</span><span class="sxs-lookup"><span data-stu-id="d19cd-106">Properties</span></span>

| <span data-ttu-id="d19cd-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="d19cd-107">Property name</span></span>              | <span data-ttu-id="d19cd-108">类型</span><span class="sxs-lookup"><span data-stu-id="d19cd-108">Type</span></span>    | <span data-ttu-id="d19cd-109">说明</span><span class="sxs-lookup"><span data-stu-id="d19cd-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="d19cd-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="d19cd-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="d19cd-111">boolean</span><span class="sxs-lookup"><span data-stu-id="d19cd-111">boolean</span></span> | <span data-ttu-id="d19cd-112">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="d19cd-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="d19cd-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="d19cd-113">**displayAs**</span></span>              | <span data-ttu-id="d19cd-114">string</span><span class="sxs-lookup"><span data-stu-id="d19cd-114">string</span></span>  | <span data-ttu-id="d19cd-115">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="d19cd-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="d19cd-116">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="d19cd-116">See below.</span></span>
| <span data-ttu-id="d19cd-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="d19cd-117">**chooseFromType**</span></span>         | <span data-ttu-id="d19cd-118">string</span><span class="sxs-lookup"><span data-stu-id="d19cd-118">string</span></span>  | <span data-ttu-id="d19cd-119">是否允许仅选择人员，或人员和组。</span><span class="sxs-lookup"><span data-stu-id="d19cd-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="d19cd-120">必须是 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="d19cd-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="d19cd-121">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="d19cd-121">DisplayAs values</span></span>

| <span data-ttu-id="d19cd-122">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="d19cd-122">DisplayAs value</span></span>               | <span data-ttu-id="d19cd-123">说明</span><span class="sxs-lookup"><span data-stu-id="d19cd-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="d19cd-124">**account**</span><span class="sxs-lookup"><span data-stu-id="d19cd-124">**Account**</span></span>                   | <span data-ttu-id="d19cd-125">个人或组的原始 SharePoint 编码的声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="d19cd-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="d19cd-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="d19cd-126">i:0#.f</span></span>|<span data-ttu-id="d19cd-127">membership</span><span class="sxs-lookup"><span data-stu-id="d19cd-127">membership</span></span>|<span data-ttu-id="d19cd-128">jane@contoso.com）。</span><span class="sxs-lookup"><span data-stu-id="d19cd-128">jane@contoso.com).</span></span>
| <span data-ttu-id="d19cd-129">**department**</span><span class="sxs-lookup"><span data-stu-id="d19cd-129">**department**</span></span>                | <span data-ttu-id="d19cd-130">个人或组所在的部门。</span><span class="sxs-lookup"><span data-stu-id="d19cd-130">The person or group's department.</span></span>
| <span data-ttu-id="d19cd-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="d19cd-131">**FirstName**</span></span>                 | <span data-ttu-id="d19cd-132">个人的名字。</span><span class="sxs-lookup"><span data-stu-id="d19cd-132">The person's given name.</span></span>
| <span data-ttu-id="d19cd-133">**id**</span><span class="sxs-lookup"><span data-stu-id="d19cd-133">**id**</span></span>                        | <span data-ttu-id="d19cd-134">目录中个人或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="d19cd-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="d19cd-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="d19cd-135">**LastName**</span></span>                  | <span data-ttu-id="d19cd-136">个人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="d19cd-136">The person's given name.</span></span>
| <span data-ttu-id="d19cd-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="d19cd-137">**mobilePhone**</span></span>               | <span data-ttu-id="d19cd-138">个人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="d19cd-138">The contact's mobile phone number.</span></span>
| <span data-ttu-id="d19cd-139">**name**</span><span class="sxs-lookup"><span data-stu-id="d19cd-139">**name**</span></span>                      | <span data-ttu-id="d19cd-140">个人的名称。</span><span class="sxs-lookup"><span data-stu-id="d19cd-140">The person's given name.</span></span>
| <span data-ttu-id="d19cd-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="d19cd-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="d19cd-142">个人的姓名及其照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="d19cd-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="d19cd-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="d19cd-143">**nameWithPresence**</span></span>          | <span data-ttu-id="d19cd-144">默认值。</span><span class="sxs-lookup"><span data-stu-id="d19cd-144">Default.</span></span> <span data-ttu-id="d19cd-145">带有状态指示器图标（空闲/忙碌等）的个人名称</span><span class="sxs-lookup"><span data-stu-id="d19cd-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="d19cd-146">**office**</span><span class="sxs-lookup"><span data-stu-id="d19cd-146">**Office**</span></span>                    | <span data-ttu-id="d19cd-147">个人的办公室号码。</span><span class="sxs-lookup"><span data-stu-id="d19cd-147">The person's office number.</span></span>
| <span data-ttu-id="d19cd-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="d19cd-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="d19cd-149">个人的照片，采用 36x36 像素的正方形边框。</span><span class="sxs-lookup"><span data-stu-id="d19cd-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="d19cd-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="d19cd-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="d19cd-151">个人的照片，采用 48x48 像素的正方形边框。</span><span class="sxs-lookup"><span data-stu-id="d19cd-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="d19cd-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="d19cd-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="d19cd-153">个人的照片，采用 72x72 像素的正方形边框。</span><span class="sxs-lookup"><span data-stu-id="d19cd-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="d19cd-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="d19cd-154">**sipAddress**</span></span>                | <span data-ttu-id="d19cd-155">个人的 SIP 地址。</span><span class="sxs-lookup"><span data-stu-id="d19cd-155">The person's sip address.</span></span>
| <span data-ttu-id="d19cd-156">**title**</span><span class="sxs-lookup"><span data-stu-id="d19cd-156">**title**</span></span>                     | <span data-ttu-id="d19cd-157">组织中的个人头衔。</span><span class="sxs-lookup"><span data-stu-id="d19cd-157">The person's title in the organization.</span></span>
| <span data-ttu-id="d19cd-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="d19cd-158">**UserName**</span></span>                  | <span data-ttu-id="d19cd-159">个人或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="d19cd-159">The person or group's user name.</span></span>
| <span data-ttu-id="d19cd-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="d19cd-160">**WorkEmail**</span></span>                 | <span data-ttu-id="d19cd-161">个人或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d19cd-161">The person or group's email address.</span></span>
| <span data-ttu-id="d19cd-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="d19cd-162">**WorkPhone**</span></span>                 | <span data-ttu-id="d19cd-163">个人的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="d19cd-163">The person's work phone number.</span></span>

<span data-ttu-id="d19cd-164">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="d19cd-164">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
