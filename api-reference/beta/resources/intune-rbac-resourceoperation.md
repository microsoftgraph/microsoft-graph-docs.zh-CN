---
title: resourceOperation 资源类型
description: 介绍 Intune，支持基于角色的访问控制 (RBAC) 的 Microsoft Graph api resourceOperation 资源。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 897c076139f3a385152738dd5f4b15c06320990d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425020"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="ad9b2-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad9b2-103">resourceOperation resource type</span></span>

> <span data-ttu-id="ad9b2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad9b2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad9b2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad9b2-107">这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-107">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="ad9b2-108">常用操作有读取、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-108">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="ad9b2-109">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-109">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="ad9b2-110">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-110">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="ad9b2-111">例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-111">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="ad9b2-112">无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-112">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="ad9b2-113">常用操作有获取、列出、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-113">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="ad9b2-114">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-114">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="ad9b2-115">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-115">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="ad9b2-116">例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-116">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="ad9b2-117">无法修改内置角色的资源操作。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-117">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="ad9b2-118">方法</span><span class="sxs-lookup"><span data-stu-id="ad9b2-118">Methods</span></span>
|<span data-ttu-id="ad9b2-119">方法</span><span class="sxs-lookup"><span data-stu-id="ad9b2-119">Method</span></span>|<span data-ttu-id="ad9b2-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="ad9b2-120">Return Type</span></span>|<span data-ttu-id="ad9b2-121">说明</span><span class="sxs-lookup"><span data-stu-id="ad9b2-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ad9b2-122">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="ad9b2-122">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="ad9b2-123">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ad9b2-123">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="ad9b2-124">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-124">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="ad9b2-125">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-125">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="ad9b2-126">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-126">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ad9b2-127">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-127">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ad9b2-128">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-128">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="ad9b2-129">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-129">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ad9b2-130">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-130">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ad9b2-131">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-131">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="ad9b2-132">无</span><span class="sxs-lookup"><span data-stu-id="ad9b2-132">None</span></span>|<span data-ttu-id="ad9b2-133">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-133">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="ad9b2-134">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-134">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="ad9b2-135">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-135">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ad9b2-136">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-136">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ad9b2-137">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="ad9b2-137">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="ad9b2-138">String collection</span><span class="sxs-lookup"><span data-stu-id="ad9b2-138">String collection</span></span>|<span data-ttu-id="ad9b2-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ad9b2-139">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ad9b2-140">属性</span><span class="sxs-lookup"><span data-stu-id="ad9b2-140">Properties</span></span>
|<span data-ttu-id="ad9b2-141">属性</span><span class="sxs-lookup"><span data-stu-id="ad9b2-141">Property</span></span>|<span data-ttu-id="ad9b2-142">类型</span><span class="sxs-lookup"><span data-stu-id="ad9b2-142">Type</span></span>|<span data-ttu-id="ad9b2-143">说明</span><span class="sxs-lookup"><span data-stu-id="ad9b2-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad9b2-144">id</span><span class="sxs-lookup"><span data-stu-id="ad9b2-144">id</span></span>|<span data-ttu-id="ad9b2-145">String</span><span class="sxs-lookup"><span data-stu-id="ad9b2-145">String</span></span>|<span data-ttu-id="ad9b2-146">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-146">Key of the Resource Operation.</span></span> <span data-ttu-id="ad9b2-147">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-147">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ad9b2-148">资源</span><span class="sxs-lookup"><span data-stu-id="ad9b2-148">resource</span></span>|<span data-ttu-id="ad9b2-149">String</span><span class="sxs-lookup"><span data-stu-id="ad9b2-149">String</span></span>|<span data-ttu-id="ad9b2-150">资源此操作所属类别。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-150">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="ad9b2-151">resourceName</span><span class="sxs-lookup"><span data-stu-id="ad9b2-151">resourceName</span></span>|<span data-ttu-id="ad9b2-152">String</span><span class="sxs-lookup"><span data-stu-id="ad9b2-152">String</span></span>|<span data-ttu-id="ad9b2-153">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-153">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ad9b2-154">actionName</span><span class="sxs-lookup"><span data-stu-id="ad9b2-154">actionName</span></span>|<span data-ttu-id="ad9b2-155">String</span><span class="sxs-lookup"><span data-stu-id="ad9b2-155">String</span></span>|<span data-ttu-id="ad9b2-156">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-156">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ad9b2-157">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-157">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ad9b2-158">说明</span><span class="sxs-lookup"><span data-stu-id="ad9b2-158">description</span></span>|<span data-ttu-id="ad9b2-159">String</span><span class="sxs-lookup"><span data-stu-id="ad9b2-159">String</span></span>|<span data-ttu-id="ad9b2-160">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-160">Description of the resource operation.</span></span> <span data-ttu-id="ad9b2-161">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-161">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="ad9b2-162">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="ad9b2-162">enabledForScopeValidation</span></span>|<span data-ttu-id="ad9b2-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad9b2-163">Boolean</span></span>|<span data-ttu-id="ad9b2-164">确定是否定义每个角色分配的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-164">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad9b2-165">关系</span><span class="sxs-lookup"><span data-stu-id="ad9b2-165">Relationships</span></span>
<span data-ttu-id="ad9b2-166">无</span><span class="sxs-lookup"><span data-stu-id="ad9b2-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad9b2-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad9b2-167">JSON Representation</span></span>
<span data-ttu-id="ad9b2-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad9b2-168">Here is a JSON representation of the resource.</span></span>
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




