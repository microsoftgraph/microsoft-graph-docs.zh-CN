---
title: identityUserFlowAttributeAssignment 资源类型
description: identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65859cb0d235454577e236761064f4597f5c68d8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158784"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="7178b-103">identityUserFlowAttributeAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7178b-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="7178b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7178b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7178b-105">identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。</span><span class="sxs-lookup"><span data-stu-id="7178b-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="7178b-106">这允许控制在用户流内收集的属性，并提供自定义选项，了解如何在用户流中收集属性。</span><span class="sxs-lookup"><span data-stu-id="7178b-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="7178b-107">您可以在单个用户流中拥有多个 identityUserFlowAttributeAssignments，该流可在要求最终用户提供用户流完成注册所需的信息时创建最终用户在注册期间看到的体验。</span><span class="sxs-lookup"><span data-stu-id="7178b-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="7178b-108">方法</span><span class="sxs-lookup"><span data-stu-id="7178b-108">Methods</span></span>

|<span data-ttu-id="7178b-109">方法</span><span class="sxs-lookup"><span data-stu-id="7178b-109">Method</span></span>|<span data-ttu-id="7178b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7178b-110">Return type</span></span>|<span data-ttu-id="7178b-111">说明</span><span class="sxs-lookup"><span data-stu-id="7178b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7178b-112">获取 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="7178b-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="7178b-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="7178b-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="7178b-114">读取 identityUserFlowAttributeAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7178b-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="7178b-115">更新 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="7178b-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="7178b-116">无</span><span class="sxs-lookup"><span data-stu-id="7178b-116">None</span></span>|<span data-ttu-id="7178b-117">更新 identityUserFlowAttributeAssignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7178b-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="7178b-118">删除 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="7178b-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="7178b-119">无</span><span class="sxs-lookup"><span data-stu-id="7178b-119">None</span></span>|<span data-ttu-id="7178b-120">删除特定 identityUserFlowAttributeAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="7178b-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="7178b-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="7178b-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="7178b-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="7178b-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="7178b-123">获取在用户流中收集的 identityUserFlowAttributes 的顺序。</span><span class="sxs-lookup"><span data-stu-id="7178b-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="7178b-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="7178b-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="7178b-125">无</span><span class="sxs-lookup"><span data-stu-id="7178b-125">None</span></span>|<span data-ttu-id="7178b-126">设置在用户流中收集的 identityUserFlowAttributes 的顺序。</span><span class="sxs-lookup"><span data-stu-id="7178b-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="7178b-127">属性</span><span class="sxs-lookup"><span data-stu-id="7178b-127">Properties</span></span>

|<span data-ttu-id="7178b-128">属性</span><span class="sxs-lookup"><span data-stu-id="7178b-128">Property</span></span>|<span data-ttu-id="7178b-129">类型</span><span class="sxs-lookup"><span data-stu-id="7178b-129">Type</span></span>|<span data-ttu-id="7178b-130">说明</span><span class="sxs-lookup"><span data-stu-id="7178b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7178b-131">id</span><span class="sxs-lookup"><span data-stu-id="7178b-131">id</span></span>|<span data-ttu-id="7178b-132">String</span><span class="sxs-lookup"><span data-stu-id="7178b-132">String</span></span>|<span data-ttu-id="7178b-133">identityUserFlowAttributeAssignment 的标识符。</span><span class="sxs-lookup"><span data-stu-id="7178b-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="7178b-134">此标识符创建后是不可可变的。</span><span class="sxs-lookup"><span data-stu-id="7178b-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="7178b-135">这是一个只读属性。</span><span class="sxs-lookup"><span data-stu-id="7178b-135">This is a read-only property.</span></span>|
|<span data-ttu-id="7178b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7178b-136">displayName</span></span>|<span data-ttu-id="7178b-137">String</span><span class="sxs-lookup"><span data-stu-id="7178b-137">String</span></span>|<span data-ttu-id="7178b-138">用户显示名称中的 identityUserFlowAttribute 的项。</span><span class="sxs-lookup"><span data-stu-id="7178b-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="7178b-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="7178b-139">isOptional</span></span>|<span data-ttu-id="7178b-140">布尔</span><span class="sxs-lookup"><span data-stu-id="7178b-140">Boolean</span></span>|<span data-ttu-id="7178b-141">确定 identityUserFlowAttribute 是否可选。</span><span class="sxs-lookup"><span data-stu-id="7178b-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="7178b-142">`true` 表示用户不必提供值。</span><span class="sxs-lookup"><span data-stu-id="7178b-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="7178b-143">`false` 表示用户无法在未提供值的情况下完成注册。</span><span class="sxs-lookup"><span data-stu-id="7178b-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="7178b-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="7178b-144">requiresVerification</span></span>|<span data-ttu-id="7178b-145">布尔</span><span class="sxs-lookup"><span data-stu-id="7178b-145">Boolean</span></span>|<span data-ttu-id="7178b-146">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="7178b-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="7178b-147">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7178b-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="7178b-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="7178b-148">userAttributeValues</span></span>|<span data-ttu-id="7178b-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7178b-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="7178b-150">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="7178b-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="7178b-151">仅在 userInputType 为 `radioSingleSelect` ，或 `dropdownSingleSelect` 时适用 `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="7178b-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="7178b-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="7178b-152">userInputType</span></span>|<span data-ttu-id="7178b-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="7178b-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="7178b-154">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="7178b-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="7178b-155">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="7178b-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7178b-156">关系</span><span class="sxs-lookup"><span data-stu-id="7178b-156">Relationships</span></span>

|<span data-ttu-id="7178b-157">关系</span><span class="sxs-lookup"><span data-stu-id="7178b-157">Relationship</span></span>|<span data-ttu-id="7178b-158">类型</span><span class="sxs-lookup"><span data-stu-id="7178b-158">Type</span></span>|<span data-ttu-id="7178b-159">说明</span><span class="sxs-lookup"><span data-stu-id="7178b-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7178b-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="7178b-160">userAttribute</span></span>|[<span data-ttu-id="7178b-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="7178b-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="7178b-162">要添加到用户流中的用户属性。</span><span class="sxs-lookup"><span data-stu-id="7178b-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7178b-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7178b-163">JSON representation</span></span>

<span data-ttu-id="7178b-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7178b-164">The following is a JSON representation of the resource.</span></span>
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
