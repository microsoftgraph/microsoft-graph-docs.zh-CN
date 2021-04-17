---
title: identityUserFlowAttributeAssignment 资源类型
description: 表示如何在标识用户流中收集属性。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0df6309682158e3d4890c6549bc7aeebb710254c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882911"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="623d8-103">identityUserFlowAttributeAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="623d8-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="623d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="623d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="623d8-105">表示如何在标识用户流中收集属性。</span><span class="sxs-lookup"><span data-stu-id="623d8-105">Represents how attributes are collected in an identity user flow.</span></span> <span data-ttu-id="623d8-106">这允许自定义选项在用户流中收集属性。</span><span class="sxs-lookup"><span data-stu-id="623d8-106">This allows customization options for collecting attributes within the user flow.</span></span> <span data-ttu-id="623d8-107">您可以在单个用户流中拥有多个 identityUserFlowAttributeAssignments，从而创建提供用户完成注册所需信息的体验。</span><span class="sxs-lookup"><span data-stu-id="623d8-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience for providing the information required by the user to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="623d8-108">方法</span><span class="sxs-lookup"><span data-stu-id="623d8-108">Methods</span></span>

|<span data-ttu-id="623d8-109">方法</span><span class="sxs-lookup"><span data-stu-id="623d8-109">Method</span></span>|<span data-ttu-id="623d8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="623d8-110">Return type</span></span>|<span data-ttu-id="623d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="623d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="623d8-112">获取 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="623d8-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="623d8-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="623d8-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="623d8-114">读取 identityUserFlowAttributeAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="623d8-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="623d8-115">更新 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="623d8-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="623d8-116">无</span><span class="sxs-lookup"><span data-stu-id="623d8-116">None</span></span>|<span data-ttu-id="623d8-117">更新 identityUserFlowAttributeAssignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="623d8-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="623d8-118">删除 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="623d8-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="623d8-119">无</span><span class="sxs-lookup"><span data-stu-id="623d8-119">None</span></span>|<span data-ttu-id="623d8-120">删除特定 identityUserFlowAttributeAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="623d8-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="623d8-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="623d8-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="623d8-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="623d8-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="623d8-123">获取在用户流中收集的 identityUserFlowAttributes 的顺序。</span><span class="sxs-lookup"><span data-stu-id="623d8-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="623d8-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="623d8-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="623d8-125">无</span><span class="sxs-lookup"><span data-stu-id="623d8-125">None</span></span>|<span data-ttu-id="623d8-126">设置在用户流中收集的 identityUserFlowAttributes 的顺序。</span><span class="sxs-lookup"><span data-stu-id="623d8-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="623d8-127">属性</span><span class="sxs-lookup"><span data-stu-id="623d8-127">Properties</span></span>

|<span data-ttu-id="623d8-128">属性</span><span class="sxs-lookup"><span data-stu-id="623d8-128">Property</span></span>|<span data-ttu-id="623d8-129">类型</span><span class="sxs-lookup"><span data-stu-id="623d8-129">Type</span></span>|<span data-ttu-id="623d8-130">说明</span><span class="sxs-lookup"><span data-stu-id="623d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623d8-131">id</span><span class="sxs-lookup"><span data-stu-id="623d8-131">id</span></span>|<span data-ttu-id="623d8-132">String</span><span class="sxs-lookup"><span data-stu-id="623d8-132">String</span></span>|<span data-ttu-id="623d8-133">identityUserFlowAttributeAssignment 的标识符。</span><span class="sxs-lookup"><span data-stu-id="623d8-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="623d8-134">此标识符创建后是不可可变的。</span><span class="sxs-lookup"><span data-stu-id="623d8-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="623d8-135">这是一个只读属性。</span><span class="sxs-lookup"><span data-stu-id="623d8-135">This is a read-only property.</span></span>|
|<span data-ttu-id="623d8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="623d8-136">displayName</span></span>|<span data-ttu-id="623d8-137">String</span><span class="sxs-lookup"><span data-stu-id="623d8-137">String</span></span>|<span data-ttu-id="623d8-138">用户显示名称中的 identityUserFlowAttribute 的组。</span><span class="sxs-lookup"><span data-stu-id="623d8-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="623d8-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="623d8-139">isOptional</span></span>|<span data-ttu-id="623d8-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="623d8-140">Boolean</span></span>|<span data-ttu-id="623d8-141">确定 identityUserFlowAttribute 是否可选。</span><span class="sxs-lookup"><span data-stu-id="623d8-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="623d8-142">`true` 表示用户不必提供值。</span><span class="sxs-lookup"><span data-stu-id="623d8-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="623d8-143">`false` 表示用户无法在未提供值的情况下完成注册。</span><span class="sxs-lookup"><span data-stu-id="623d8-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="623d8-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="623d8-144">requiresVerification</span></span>|<span data-ttu-id="623d8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="623d8-145">Boolean</span></span>|<span data-ttu-id="623d8-146">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="623d8-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="623d8-147">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="623d8-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="623d8-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="623d8-148">userAttributeValues</span></span>|<span data-ttu-id="623d8-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="623d8-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="623d8-150">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="623d8-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="623d8-151">仅在 userInputType 为 `radioSingleSelect` 、 `dropdownSingleSelect` 或 时适用 `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="623d8-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="623d8-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="623d8-152">userInputType</span></span>|<span data-ttu-id="623d8-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="623d8-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="623d8-154">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="623d8-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="623d8-155">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="623d8-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="623d8-156">关系</span><span class="sxs-lookup"><span data-stu-id="623d8-156">Relationships</span></span>

|<span data-ttu-id="623d8-157">关系</span><span class="sxs-lookup"><span data-stu-id="623d8-157">Relationship</span></span>|<span data-ttu-id="623d8-158">类型</span><span class="sxs-lookup"><span data-stu-id="623d8-158">Type</span></span>|<span data-ttu-id="623d8-159">说明</span><span class="sxs-lookup"><span data-stu-id="623d8-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623d8-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="623d8-160">userAttribute</span></span>|[<span data-ttu-id="623d8-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="623d8-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="623d8-162">要添加到用户流的用户属性。</span><span class="sxs-lookup"><span data-stu-id="623d8-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="623d8-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="623d8-163">JSON representation</span></span>

<span data-ttu-id="623d8-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="623d8-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
  "id": "String (identifier)",
  "isOptional": "Boolean",
  "requiresVerification": "Boolean",
  "userInputType": "String",
  "userAttributeValues": [
    {
      "@odata.type": "microsoft.graph.userAttributeValuesItem"
    }
  ],
  "displayName": "String"
}
```
