---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: b0c6eab7d2111870192a4ed6c30c1cbd72e4163e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010392"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="6fec8-102">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fec8-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="6fec8-103">[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="6fec8-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fec8-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fec8-104">JSON representation</span></span>

<span data-ttu-id="6fec8-105">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fec8-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="6fec8-106">属性</span><span class="sxs-lookup"><span data-stu-id="6fec8-106">Properties</span></span>

| <span data-ttu-id="6fec8-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="6fec8-107">Property name</span></span>              | <span data-ttu-id="6fec8-108">类型</span><span class="sxs-lookup"><span data-stu-id="6fec8-108">Type</span></span>    | <span data-ttu-id="6fec8-109">说明</span><span class="sxs-lookup"><span data-stu-id="6fec8-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="6fec8-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="6fec8-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="6fec8-111">boolean</span><span class="sxs-lookup"><span data-stu-id="6fec8-111">boolean</span></span> | <span data-ttu-id="6fec8-112">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="6fec8-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="6fec8-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="6fec8-113">**displayAs**</span></span>              | <span data-ttu-id="6fec8-114">string</span><span class="sxs-lookup"><span data-stu-id="6fec8-114">string</span></span>  | <span data-ttu-id="6fec8-115">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="6fec8-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="6fec8-116">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="6fec8-116">See below.</span></span>
| <span data-ttu-id="6fec8-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="6fec8-117">**chooseFromType**</span></span>         | <span data-ttu-id="6fec8-118">string</span><span class="sxs-lookup"><span data-stu-id="6fec8-118">string</span></span>  | <span data-ttu-id="6fec8-119">是否允许仅选择人员，或同时选择人员和组。</span><span class="sxs-lookup"><span data-stu-id="6fec8-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="6fec8-120">必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="6fec8-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="6fec8-121">DisplayAs 选项</span><span class="sxs-lookup"><span data-stu-id="6fec8-121">DisplayAs options</span></span>

| <span data-ttu-id="6fec8-122">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="6fec8-122">DisplayAs value</span></span>               | <span data-ttu-id="6fec8-123">说明</span><span class="sxs-lookup"><span data-stu-id="6fec8-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="6fec8-124">**帐户**</span><span class="sxs-lookup"><span data-stu-id="6fec8-124">**account**</span></span>                   | <span data-ttu-id="6fec8-125">采用原始 SharePoint 编码的人员或组声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="6fec8-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="6fec8-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="6fec8-126">i:0#.f</span></span>|<span data-ttu-id="6fec8-127">membership</span><span class="sxs-lookup"><span data-stu-id="6fec8-127">membership</span></span>|<span data-ttu-id="6fec8-128">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="6fec8-128">jane@contoso.com).</span></span>
| <span data-ttu-id="6fec8-129">**department**</span><span class="sxs-lookup"><span data-stu-id="6fec8-129">**department**</span></span>                | <span data-ttu-id="6fec8-130">人员或组的所在部门。</span><span class="sxs-lookup"><span data-stu-id="6fec8-130">The person or group's department.</span></span>
| <span data-ttu-id="6fec8-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="6fec8-131">**firstName**</span></span>                 | <span data-ttu-id="6fec8-132">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="6fec8-132">The person's first name.</span></span>
| <span data-ttu-id="6fec8-133">**id**</span><span class="sxs-lookup"><span data-stu-id="6fec8-133">**id**</span></span>                        | <span data-ttu-id="6fec8-134">目录中个人或组的 id。</span><span class="sxs-lookup"><span data-stu-id="6fec8-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="6fec8-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="6fec8-135">**lastName**</span></span>                  | <span data-ttu-id="6fec8-136">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="6fec8-136">The person's last name.</span></span>
| <span data-ttu-id="6fec8-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="6fec8-137">**mobilePhone**</span></span>               | <span data-ttu-id="6fec8-138">人员的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="6fec8-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="6fec8-139">**name**</span><span class="sxs-lookup"><span data-stu-id="6fec8-139">**name**</span></span>                      | <span data-ttu-id="6fec8-140">人员姓名。</span><span class="sxs-lookup"><span data-stu-id="6fec8-140">The person's name.</span></span>
| <span data-ttu-id="6fec8-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="6fec8-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="6fec8-142">人员姓名，以及他们的照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fec8-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="6fec8-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="6fec8-143">**nameWithPresence**</span></span>          | <span data-ttu-id="6fec8-144">默认值。</span><span class="sxs-lookup"><span data-stu-id="6fec8-144">Default.</span></span> <span data-ttu-id="6fec8-145">人员姓名和状态指示器图标（空闲/忙碌/等）</span><span class="sxs-lookup"><span data-stu-id="6fec8-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="6fec8-146">**office**</span><span class="sxs-lookup"><span data-stu-id="6fec8-146">**office**</span></span>                    | <span data-ttu-id="6fec8-147">人员的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="6fec8-147">The person's office number.</span></span>
| <span data-ttu-id="6fec8-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="6fec8-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="6fec8-149">人员的照片，采用 36x36 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="6fec8-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="6fec8-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="6fec8-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="6fec8-151">人员的照片，采用 48x48 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="6fec8-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="6fec8-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="6fec8-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="6fec8-153">人员的照片，采用 72x72 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="6fec8-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="6fec8-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="6fec8-154">**sipAddress**</span></span>                | <span data-ttu-id="6fec8-155">人员的 sip 地址。</span><span class="sxs-lookup"><span data-stu-id="6fec8-155">The person's sip address.</span></span>
| <span data-ttu-id="6fec8-156">**title**</span><span class="sxs-lookup"><span data-stu-id="6fec8-156">**title**</span></span>                     | <span data-ttu-id="6fec8-157">人员在组织中的职务。</span><span class="sxs-lookup"><span data-stu-id="6fec8-157">The person's title in the organization.</span></span>
| <span data-ttu-id="6fec8-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="6fec8-158">**userName**</span></span>                  | <span data-ttu-id="6fec8-159">人员或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="6fec8-159">The person or group's user name.</span></span>
| <span data-ttu-id="6fec8-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="6fec8-160">**workEmail**</span></span>                 | <span data-ttu-id="6fec8-161">人员或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6fec8-161">The person or group's email address.</span></span>
| <span data-ttu-id="6fec8-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="6fec8-162">**workPhone**</span></span>                 | <span data-ttu-id="6fec8-163">人员的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="6fec8-163">The person's work phone number.</span></span>

<span data-ttu-id="6fec8-164">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="6fec8-164">Note: Additional DisplayAs types may be returned.</span></span>

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
