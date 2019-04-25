---
title: resourceOperation 资源类型
description: 这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。  常用操作有读取、删除、更新或创建。  这些操作提供对基础 Intune 资源本身的基本管理。  某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。  例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。  无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。  常用操作有获取、列出、删除、更新或创建。  这些操作提供对基础 Intune 资源本身的基本管理。  某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。  例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。  无法修改内置角色的资源操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f2ccbf60dffa6f8f0fafd6cfc4238b57e1d17c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573100"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="b39f8-113">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b39f8-113">resourceOperation resource type</span></span>

> <span data-ttu-id="b39f8-114">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b39f8-114">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b39f8-115">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b39f8-115">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b39f8-116">这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="b39f8-116">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="b39f8-117">常用操作有读取、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="b39f8-117">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="b39f8-118">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="b39f8-118">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="b39f8-119">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="b39f8-119">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="b39f8-120">例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="b39f8-120">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="b39f8-121">无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="b39f8-121">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="b39f8-122">常用操作有获取、列出、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="b39f8-122">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="b39f8-123">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="b39f8-123">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="b39f8-124">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="b39f8-124">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="b39f8-125">例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="b39f8-125">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="b39f8-126">无法修改内置角色的资源操作。</span><span class="sxs-lookup"><span data-stu-id="b39f8-126">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="b39f8-127">方法</span><span class="sxs-lookup"><span data-stu-id="b39f8-127">Methods</span></span>
|<span data-ttu-id="b39f8-128">方法</span><span class="sxs-lookup"><span data-stu-id="b39f8-128">Method</span></span>|<span data-ttu-id="b39f8-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="b39f8-129">Return Type</span></span>|<span data-ttu-id="b39f8-130">说明</span><span class="sxs-lookup"><span data-stu-id="b39f8-130">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b39f8-131">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="b39f8-131">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="b39f8-132">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b39f8-132">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="b39f8-133">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b39f8-133">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="b39f8-134">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-134">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="b39f8-135">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-135">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="b39f8-136">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b39f8-136">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="b39f8-137">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-137">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="b39f8-138">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-138">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="b39f8-139">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b39f8-139">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="b39f8-140">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-140">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="b39f8-141">无</span><span class="sxs-lookup"><span data-stu-id="b39f8-141">None</span></span>|<span data-ttu-id="b39f8-142">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="b39f8-142">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="b39f8-143">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-143">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="b39f8-144">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="b39f8-144">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="b39f8-145">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b39f8-145">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="b39f8-146">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="b39f8-146">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="b39f8-147">String collection</span><span class="sxs-lookup"><span data-stu-id="b39f8-147">String collection</span></span>|<span data-ttu-id="b39f8-148">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b39f8-148">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b39f8-149">属性</span><span class="sxs-lookup"><span data-stu-id="b39f8-149">Properties</span></span>
|<span data-ttu-id="b39f8-150">属性</span><span class="sxs-lookup"><span data-stu-id="b39f8-150">Property</span></span>|<span data-ttu-id="b39f8-151">类型</span><span class="sxs-lookup"><span data-stu-id="b39f8-151">Type</span></span>|<span data-ttu-id="b39f8-152">说明</span><span class="sxs-lookup"><span data-stu-id="b39f8-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39f8-153">id</span><span class="sxs-lookup"><span data-stu-id="b39f8-153">id</span></span>|<span data-ttu-id="b39f8-154">字符串</span><span class="sxs-lookup"><span data-stu-id="b39f8-154">String</span></span>|<span data-ttu-id="b39f8-155">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="b39f8-155">Key of the Resource Operation.</span></span> <span data-ttu-id="b39f8-156">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="b39f8-156">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="b39f8-157">资源</span><span class="sxs-lookup"><span data-stu-id="b39f8-157">resource</span></span>|<span data-ttu-id="b39f8-158">String</span><span class="sxs-lookup"><span data-stu-id="b39f8-158">String</span></span>|<span data-ttu-id="b39f8-159">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="b39f8-159">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="b39f8-160">resourceName</span><span class="sxs-lookup"><span data-stu-id="b39f8-160">resourceName</span></span>|<span data-ttu-id="b39f8-161">String</span><span class="sxs-lookup"><span data-stu-id="b39f8-161">String</span></span>|<span data-ttu-id="b39f8-162">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="b39f8-162">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="b39f8-163">actionName</span><span class="sxs-lookup"><span data-stu-id="b39f8-163">actionName</span></span>|<span data-ttu-id="b39f8-164">String</span><span class="sxs-lookup"><span data-stu-id="b39f8-164">String</span></span>|<span data-ttu-id="b39f8-165">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="b39f8-165">Type of action this operation is going to perform.</span></span> <span data-ttu-id="b39f8-166">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="b39f8-166">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="b39f8-167">说明</span><span class="sxs-lookup"><span data-stu-id="b39f8-167">description</span></span>|<span data-ttu-id="b39f8-168">String</span><span class="sxs-lookup"><span data-stu-id="b39f8-168">String</span></span>|<span data-ttu-id="b39f8-169">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="b39f8-169">Description of the resource operation.</span></span> <span data-ttu-id="b39f8-170">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="b39f8-170">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="b39f8-171">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="b39f8-171">enabledForScopeValidation</span></span>|<span data-ttu-id="b39f8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39f8-172">Boolean</span></span>|<span data-ttu-id="b39f8-173">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="b39f8-173">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b39f8-174">关系</span><span class="sxs-lookup"><span data-stu-id="b39f8-174">Relationships</span></span>
<span data-ttu-id="b39f8-175">无</span><span class="sxs-lookup"><span data-stu-id="b39f8-175">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b39f8-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b39f8-176">JSON Representation</span></span>
<span data-ttu-id="b39f8-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b39f8-177">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```





