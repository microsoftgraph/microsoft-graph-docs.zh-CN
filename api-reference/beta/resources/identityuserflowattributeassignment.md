---
title: identityUserFlowAttributeAssignment 资源类型
description: identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80bc6547307914e0d206ea9b5c79073f96fce19c
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581291"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="3069c-103">identityUserFlowAttributeAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3069c-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="3069c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3069c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3069c-105">identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。</span><span class="sxs-lookup"><span data-stu-id="3069c-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="3069c-106">这允许控制在用户流中收集的属性，并提供有关如何在用户流中收集属性的自定义选项。</span><span class="sxs-lookup"><span data-stu-id="3069c-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="3069c-107">您可以在单个用户流中拥有多个 identityUserFlowAttributeAssignments，以创建最终用户在注册过程中看到的体验，如果要求提供用户流完成注册所需的信息。</span><span class="sxs-lookup"><span data-stu-id="3069c-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="3069c-108">方法</span><span class="sxs-lookup"><span data-stu-id="3069c-108">Methods</span></span>

|<span data-ttu-id="3069c-109">方法</span><span class="sxs-lookup"><span data-stu-id="3069c-109">Method</span></span>|<span data-ttu-id="3069c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3069c-110">Return type</span></span>|<span data-ttu-id="3069c-111">Description</span><span class="sxs-lookup"><span data-stu-id="3069c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3069c-112">获取 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3069c-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="3069c-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3069c-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="3069c-114">读取 identityUserFlowAttributeAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3069c-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="3069c-115">更新 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3069c-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="3069c-116">无</span><span class="sxs-lookup"><span data-stu-id="3069c-116">None</span></span>|<span data-ttu-id="3069c-117">更新 identityUserFlowAttributeAssignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3069c-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="3069c-118">删除 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3069c-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="3069c-119">无</span><span class="sxs-lookup"><span data-stu-id="3069c-119">None</span></span>|<span data-ttu-id="3069c-120">删除特定的 identityUserFlowAttributeAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="3069c-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="3069c-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="3069c-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="3069c-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="3069c-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="3069c-123">获取在用户流中收集的 identityUserFlowAttributes 的顺序。</span><span class="sxs-lookup"><span data-stu-id="3069c-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="3069c-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="3069c-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="3069c-125">无</span><span class="sxs-lookup"><span data-stu-id="3069c-125">None</span></span>|<span data-ttu-id="3069c-126">设置在用户流中收集的 identityUserFlowAttributes 的顺序。</span><span class="sxs-lookup"><span data-stu-id="3069c-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="3069c-127">属性</span><span class="sxs-lookup"><span data-stu-id="3069c-127">Properties</span></span>

|<span data-ttu-id="3069c-128">属性</span><span class="sxs-lookup"><span data-stu-id="3069c-128">Property</span></span>|<span data-ttu-id="3069c-129">类型</span><span class="sxs-lookup"><span data-stu-id="3069c-129">Type</span></span>|<span data-ttu-id="3069c-130">说明</span><span class="sxs-lookup"><span data-stu-id="3069c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3069c-131">id</span><span class="sxs-lookup"><span data-stu-id="3069c-131">id</span></span>|<span data-ttu-id="3069c-132">String</span><span class="sxs-lookup"><span data-stu-id="3069c-132">String</span></span>|<span data-ttu-id="3069c-133">IdentityUserFlowAttributeAssignment 的标识符。</span><span class="sxs-lookup"><span data-stu-id="3069c-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="3069c-134">此标识符在创建后是不可变的。</span><span class="sxs-lookup"><span data-stu-id="3069c-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="3069c-135">这是一个只读属性。</span><span class="sxs-lookup"><span data-stu-id="3069c-135">This is a read-only property.</span></span>|
|<span data-ttu-id="3069c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3069c-136">displayName</span></span>|<span data-ttu-id="3069c-137">String</span><span class="sxs-lookup"><span data-stu-id="3069c-137">String</span></span>|<span data-ttu-id="3069c-138">用户流中的 identityUserFlowAttribute 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3069c-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="3069c-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="3069c-139">isOptional</span></span>|<span data-ttu-id="3069c-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="3069c-140">Boolean</span></span>|<span data-ttu-id="3069c-141">确定 identityUserFlowAttribute 是否为可选。</span><span class="sxs-lookup"><span data-stu-id="3069c-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="3069c-142">`true` 表示用户不必提供值。</span><span class="sxs-lookup"><span data-stu-id="3069c-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="3069c-143">`false` 表示用户无法完成注册，而无需提供值。</span><span class="sxs-lookup"><span data-stu-id="3069c-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="3069c-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="3069c-144">requiresVerification</span></span>|<span data-ttu-id="3069c-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="3069c-145">Boolean</span></span>|<span data-ttu-id="3069c-146">确定 identityUserFlowAttribute 是否需要验证。</span><span class="sxs-lookup"><span data-stu-id="3069c-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="3069c-147">这仅用于验证用户的电话号码或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3069c-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="3069c-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="3069c-148">userAttributeValues</span></span>|<span data-ttu-id="3069c-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3069c-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="3069c-150">用户流属性的输入选项。</span><span class="sxs-lookup"><span data-stu-id="3069c-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="3069c-151">仅当 userInputType 为、或时才适用 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` 。</span><span class="sxs-lookup"><span data-stu-id="3069c-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="3069c-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="3069c-152">userInputType</span></span>|<span data-ttu-id="3069c-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="3069c-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="3069c-154">用户流属性的输入类型。</span><span class="sxs-lookup"><span data-stu-id="3069c-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="3069c-155">可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。</span><span class="sxs-lookup"><span data-stu-id="3069c-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3069c-156">关系</span><span class="sxs-lookup"><span data-stu-id="3069c-156">Relationships</span></span>

|<span data-ttu-id="3069c-157">关系</span><span class="sxs-lookup"><span data-stu-id="3069c-157">Relationship</span></span>|<span data-ttu-id="3069c-158">类型</span><span class="sxs-lookup"><span data-stu-id="3069c-158">Type</span></span>|<span data-ttu-id="3069c-159">Description</span><span class="sxs-lookup"><span data-stu-id="3069c-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3069c-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="3069c-160">userAttribute</span></span>|[<span data-ttu-id="3069c-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="3069c-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="3069c-162">要添加到用户流中的用户属性。</span><span class="sxs-lookup"><span data-stu-id="3069c-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3069c-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3069c-163">JSON representation</span></span>

<span data-ttu-id="3069c-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3069c-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "baseType": "",
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
