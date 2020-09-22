---
title: resourceOperation 资源类型
description: 描述 resourceOperation 资源 (entity) of Microsoft Graph API (REST) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8936fd112001b33f977a7cd60dce892c8983083
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056511"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="929cd-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="929cd-103">resourceOperation resource type</span></span>

<span data-ttu-id="929cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="929cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="929cd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="929cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="929cd-106">这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="929cd-106">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="929cd-107">常用操作有读取、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="929cd-107">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="929cd-108">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="929cd-108">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="929cd-109">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="929cd-109">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="929cd-110">例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="929cd-110">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="929cd-111">无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="929cd-111">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="929cd-112">常用操作有获取、列出、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="929cd-112">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="929cd-113">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="929cd-113">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="929cd-114">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="929cd-114">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="929cd-115">例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="929cd-115">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="929cd-116">无法修改内置角色的资源操作。</span><span class="sxs-lookup"><span data-stu-id="929cd-116">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="929cd-117">方法</span><span class="sxs-lookup"><span data-stu-id="929cd-117">Methods</span></span>
|<span data-ttu-id="929cd-118">方法</span><span class="sxs-lookup"><span data-stu-id="929cd-118">Method</span></span>|<span data-ttu-id="929cd-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="929cd-119">Return Type</span></span>|<span data-ttu-id="929cd-120">说明</span><span class="sxs-lookup"><span data-stu-id="929cd-120">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="929cd-121">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="929cd-121">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="929cd-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="929cd-122">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="929cd-123">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="929cd-123">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="929cd-124">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-124">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="929cd-125">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-125">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="929cd-126">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="929cd-126">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="929cd-127">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-127">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="929cd-128">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-128">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="929cd-129">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="929cd-129">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="929cd-130">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-130">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="929cd-131">无</span><span class="sxs-lookup"><span data-stu-id="929cd-131">None</span></span>|<span data-ttu-id="929cd-132">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="929cd-132">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="929cd-133">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-133">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="929cd-134">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="929cd-134">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="929cd-135">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="929cd-135">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="929cd-136">属性</span><span class="sxs-lookup"><span data-stu-id="929cd-136">Properties</span></span>
|<span data-ttu-id="929cd-137">属性</span><span class="sxs-lookup"><span data-stu-id="929cd-137">Property</span></span>|<span data-ttu-id="929cd-138">类型</span><span class="sxs-lookup"><span data-stu-id="929cd-138">Type</span></span>|<span data-ttu-id="929cd-139">说明</span><span class="sxs-lookup"><span data-stu-id="929cd-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="929cd-140">id</span><span class="sxs-lookup"><span data-stu-id="929cd-140">id</span></span>|<span data-ttu-id="929cd-141">String</span><span class="sxs-lookup"><span data-stu-id="929cd-141">String</span></span>|<span data-ttu-id="929cd-142">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="929cd-142">Key of the Resource Operation.</span></span> <span data-ttu-id="929cd-143">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="929cd-143">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="929cd-144">resourceName</span><span class="sxs-lookup"><span data-stu-id="929cd-144">resourceName</span></span>|<span data-ttu-id="929cd-145">String</span><span class="sxs-lookup"><span data-stu-id="929cd-145">String</span></span>|<span data-ttu-id="929cd-146">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="929cd-146">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="929cd-147">actionName</span><span class="sxs-lookup"><span data-stu-id="929cd-147">actionName</span></span>|<span data-ttu-id="929cd-148">String</span><span class="sxs-lookup"><span data-stu-id="929cd-148">String</span></span>|<span data-ttu-id="929cd-149">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="929cd-149">Type of action this operation is going to perform.</span></span> <span data-ttu-id="929cd-150">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="929cd-150">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="929cd-151">description</span><span class="sxs-lookup"><span data-stu-id="929cd-151">description</span></span>|<span data-ttu-id="929cd-152">String</span><span class="sxs-lookup"><span data-stu-id="929cd-152">String</span></span>|<span data-ttu-id="929cd-153">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="929cd-153">Description of the resource operation.</span></span> <span data-ttu-id="929cd-154">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="929cd-154">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="929cd-155">关系</span><span class="sxs-lookup"><span data-stu-id="929cd-155">Relationships</span></span>
<span data-ttu-id="929cd-156">无</span><span class="sxs-lookup"><span data-stu-id="929cd-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="929cd-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="929cd-157">JSON Representation</span></span>
<span data-ttu-id="929cd-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="929cd-158">Here is a JSON representation of the resource.</span></span>
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
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```









