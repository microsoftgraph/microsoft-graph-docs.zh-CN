---
title: resourceOperation 资源类型
description: 介绍适用于 Intune (REST) 的 Microsoft Graph API 的 resourceoperation 资源 (实体), 它支持租户组织的基于角色的访问控制 (RBAC) 方案。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a299247815993a6ac1e99fe11ecead7ab66e2f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165000"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="ebd1d-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebd1d-103">resourceOperation resource type</span></span>

> <span data-ttu-id="ebd1d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebd1d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd1d-106">这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-106">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="ebd1d-107">常用操作有读取、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-107">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="ebd1d-108">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-108">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="ebd1d-109">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-109">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="ebd1d-110">例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-110">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="ebd1d-111">无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-111">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="ebd1d-112">常用操作有获取、列出、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-112">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="ebd1d-113">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-113">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="ebd1d-114">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-114">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="ebd1d-115">例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-115">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="ebd1d-116">无法修改内置角色的资源操作。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-116">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="ebd1d-117">方法</span><span class="sxs-lookup"><span data-stu-id="ebd1d-117">Methods</span></span>
|<span data-ttu-id="ebd1d-118">方法</span><span class="sxs-lookup"><span data-stu-id="ebd1d-118">Method</span></span>|<span data-ttu-id="ebd1d-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebd1d-119">Return Type</span></span>|<span data-ttu-id="ebd1d-120">说明</span><span class="sxs-lookup"><span data-stu-id="ebd1d-120">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebd1d-121">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="ebd1d-121">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="ebd1d-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebd1d-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="ebd1d-123">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-123">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="ebd1d-124">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-124">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="ebd1d-125">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-125">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ebd1d-126">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-126">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ebd1d-127">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-127">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="ebd1d-128">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-128">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ebd1d-129">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-129">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ebd1d-130">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-130">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="ebd1d-131">无</span><span class="sxs-lookup"><span data-stu-id="ebd1d-131">None</span></span>|<span data-ttu-id="ebd1d-132">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-132">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="ebd1d-133">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-133">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="ebd1d-134">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-134">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ebd1d-135">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-135">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ebd1d-136">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="ebd1d-136">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="ebd1d-137">String collection</span><span class="sxs-lookup"><span data-stu-id="ebd1d-137">String collection</span></span>|<span data-ttu-id="ebd1d-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ebd1d-138">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ebd1d-139">属性</span><span class="sxs-lookup"><span data-stu-id="ebd1d-139">Properties</span></span>
|<span data-ttu-id="ebd1d-140">属性</span><span class="sxs-lookup"><span data-stu-id="ebd1d-140">Property</span></span>|<span data-ttu-id="ebd1d-141">类型</span><span class="sxs-lookup"><span data-stu-id="ebd1d-141">Type</span></span>|<span data-ttu-id="ebd1d-142">说明</span><span class="sxs-lookup"><span data-stu-id="ebd1d-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd1d-143">id</span><span class="sxs-lookup"><span data-stu-id="ebd1d-143">id</span></span>|<span data-ttu-id="ebd1d-144">字符串</span><span class="sxs-lookup"><span data-stu-id="ebd1d-144">String</span></span>|<span data-ttu-id="ebd1d-145">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-145">Key of the Resource Operation.</span></span> <span data-ttu-id="ebd1d-146">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-146">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ebd1d-147">resource</span><span class="sxs-lookup"><span data-stu-id="ebd1d-147">resource</span></span>|<span data-ttu-id="ebd1d-148">String</span><span class="sxs-lookup"><span data-stu-id="ebd1d-148">String</span></span>|<span data-ttu-id="ebd1d-149">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-149">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="ebd1d-150">resourceName</span><span class="sxs-lookup"><span data-stu-id="ebd1d-150">resourceName</span></span>|<span data-ttu-id="ebd1d-151">String</span><span class="sxs-lookup"><span data-stu-id="ebd1d-151">String</span></span>|<span data-ttu-id="ebd1d-152">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-152">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ebd1d-153">actionName</span><span class="sxs-lookup"><span data-stu-id="ebd1d-153">actionName</span></span>|<span data-ttu-id="ebd1d-154">String</span><span class="sxs-lookup"><span data-stu-id="ebd1d-154">String</span></span>|<span data-ttu-id="ebd1d-155">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-155">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ebd1d-156">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-156">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ebd1d-157">说明</span><span class="sxs-lookup"><span data-stu-id="ebd1d-157">description</span></span>|<span data-ttu-id="ebd1d-158">String</span><span class="sxs-lookup"><span data-stu-id="ebd1d-158">String</span></span>|<span data-ttu-id="ebd1d-159">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-159">Description of the resource operation.</span></span> <span data-ttu-id="ebd1d-160">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-160">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="ebd1d-161">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="ebd1d-161">enabledForScopeValidation</span></span>|<span data-ttu-id="ebd1d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1d-162">Boolean</span></span>|<span data-ttu-id="ebd1d-163">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-163">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd1d-164">关系</span><span class="sxs-lookup"><span data-stu-id="ebd1d-164">Relationships</span></span>
<span data-ttu-id="ebd1d-165">无</span><span class="sxs-lookup"><span data-stu-id="ebd1d-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebd1d-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebd1d-166">JSON Representation</span></span>
<span data-ttu-id="ebd1d-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-167">Here is a JSON representation of the resource.</span></span>
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




