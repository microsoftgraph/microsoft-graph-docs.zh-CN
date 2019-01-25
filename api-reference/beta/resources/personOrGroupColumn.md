---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a3136d7c5b9563999eb9b21a9235317afdaeb63e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519295"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="89202-102">PersonOrGroupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="89202-102">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89202-103">[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。</span><span class="sxs-lookup"><span data-stu-id="89202-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89202-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89202-104">JSON representation</span></span>

<span data-ttu-id="89202-105">下面是 **personOrGroupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89202-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="89202-106">属性</span><span class="sxs-lookup"><span data-stu-id="89202-106">Properties</span></span>

| <span data-ttu-id="89202-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="89202-107">Property name</span></span>              | <span data-ttu-id="89202-108">类型</span><span class="sxs-lookup"><span data-stu-id="89202-108">Type</span></span>    | <span data-ttu-id="89202-109">说明</span><span class="sxs-lookup"><span data-stu-id="89202-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="89202-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="89202-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="89202-111">boolean</span><span class="sxs-lookup"><span data-stu-id="89202-111">boolean</span></span> | <span data-ttu-id="89202-112">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="89202-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="89202-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="89202-113">**displayAs**</span></span>              | <span data-ttu-id="89202-114">string</span><span class="sxs-lookup"><span data-stu-id="89202-114">string</span></span>  | <span data-ttu-id="89202-115">如何显示有关所选个人或组的信息。</span><span class="sxs-lookup"><span data-stu-id="89202-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="89202-116">请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="89202-116">See below.</span></span>
| <span data-ttu-id="89202-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="89202-117">**chooseFromType**</span></span>         | <span data-ttu-id="89202-118">string</span><span class="sxs-lookup"><span data-stu-id="89202-118">string</span></span>  | <span data-ttu-id="89202-119">是否允许仅选择人员，或同时选择人员和组。</span><span class="sxs-lookup"><span data-stu-id="89202-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="89202-120">必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="89202-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="89202-121">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="89202-121">DisplayAs values</span></span>

| <span data-ttu-id="89202-122">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="89202-122">DisplayAs value</span></span>               | <span data-ttu-id="89202-123">说明</span><span class="sxs-lookup"><span data-stu-id="89202-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="89202-124">**帐户**</span><span class="sxs-lookup"><span data-stu-id="89202-124">**account**</span></span>                   | <span data-ttu-id="89202-125">采用原始 SharePoint 编码的人员或组声明字符串（如</span><span class="sxs-lookup"><span data-stu-id="89202-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="89202-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="89202-126">i:0#.f</span></span>|<span data-ttu-id="89202-127">membership</span><span class="sxs-lookup"><span data-stu-id="89202-127">membership</span></span>|<span data-ttu-id="89202-128">jane@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="89202-128">jane@contoso.com).</span></span>
| <span data-ttu-id="89202-129">**department**</span><span class="sxs-lookup"><span data-stu-id="89202-129">**department**</span></span>                | <span data-ttu-id="89202-130">人员或组的所在部门。</span><span class="sxs-lookup"><span data-stu-id="89202-130">The person or group's department.</span></span>
| <span data-ttu-id="89202-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="89202-131">**firstName**</span></span>                 | <span data-ttu-id="89202-132">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="89202-132">The person's first name.</span></span>
| <span data-ttu-id="89202-133">**id**</span><span class="sxs-lookup"><span data-stu-id="89202-133">**id**</span></span>                        | <span data-ttu-id="89202-134">目录中个人或组的 id。</span><span class="sxs-lookup"><span data-stu-id="89202-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="89202-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="89202-135">**lastName**</span></span>                  | <span data-ttu-id="89202-136">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="89202-136">The person's last name.</span></span>
| <span data-ttu-id="89202-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="89202-137">**mobilePhone**</span></span>               | <span data-ttu-id="89202-138">人员的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="89202-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="89202-139">**name**</span><span class="sxs-lookup"><span data-stu-id="89202-139">**name**</span></span>                      | <span data-ttu-id="89202-140">人员姓名。</span><span class="sxs-lookup"><span data-stu-id="89202-140">The person's name.</span></span>
| <span data-ttu-id="89202-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="89202-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="89202-142">人员姓名，以及他们的照片和其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="89202-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="89202-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="89202-143">**nameWithPresence**</span></span>          | <span data-ttu-id="89202-144">默认值。</span><span class="sxs-lookup"><span data-stu-id="89202-144">Default.</span></span> <span data-ttu-id="89202-145">人员姓名和状态指示器图标（空闲/忙碌/等）</span><span class="sxs-lookup"><span data-stu-id="89202-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="89202-146">**office**</span><span class="sxs-lookup"><span data-stu-id="89202-146">**office**</span></span>                    | <span data-ttu-id="89202-147">人员的办公室电话。</span><span class="sxs-lookup"><span data-stu-id="89202-147">The person's office number.</span></span>
| <span data-ttu-id="89202-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="89202-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="89202-149">人员的照片，采用 36x36 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="89202-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="89202-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="89202-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="89202-151">人员的照片，采用 48x48 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="89202-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="89202-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="89202-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="89202-153">人员的照片，采用 72x72 像素的正方形框。</span><span class="sxs-lookup"><span data-stu-id="89202-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="89202-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="89202-154">**sipAddress**</span></span>                | <span data-ttu-id="89202-155">人员的 sip 地址。</span><span class="sxs-lookup"><span data-stu-id="89202-155">The person's sip address.</span></span>
| <span data-ttu-id="89202-156">**title**</span><span class="sxs-lookup"><span data-stu-id="89202-156">**title**</span></span>                     | <span data-ttu-id="89202-157">人员在组织中的职务。</span><span class="sxs-lookup"><span data-stu-id="89202-157">The person's title in the organization.</span></span>
| <span data-ttu-id="89202-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="89202-158">**userName**</span></span>                  | <span data-ttu-id="89202-159">人员或组的用户名。</span><span class="sxs-lookup"><span data-stu-id="89202-159">The person or group's user name.</span></span>
| <span data-ttu-id="89202-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="89202-160">**workEmail**</span></span>                 | <span data-ttu-id="89202-161">人员或组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="89202-161">The person or group's email address.</span></span>
| <span data-ttu-id="89202-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="89202-162">**workPhone**</span></span>                 | <span data-ttu-id="89202-163">人员的工作电话号码。</span><span class="sxs-lookup"><span data-stu-id="89202-163">The person's work phone number.</span></span>

<span data-ttu-id="89202-164">注意：可能返回其他 DisplayAs 类型。</span><span class="sxs-lookup"><span data-stu-id="89202-164">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/personOrGroupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
