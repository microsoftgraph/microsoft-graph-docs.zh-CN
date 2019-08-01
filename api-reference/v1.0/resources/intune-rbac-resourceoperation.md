---
title: resourceOperation 资源类型
description: 介绍 Microsoft Graph API (REST) 的 resourceOperation 资源 (实体), 它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f3519255524c38d75b941461682f2538a6ee39a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037133"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="8e4ef-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e4ef-103">resourceOperation resource type</span></span>

> <span data-ttu-id="8e4ef-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e4ef-105">这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-105">This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="8e4ef-106">常用操作有读取、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-106">Common operations are Read, Delete, Update or Create.</span></span>  <span data-ttu-id="8e4ef-107">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-107">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="8e4ef-108">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-108">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="8e4ef-109">例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-109">For example, the Assign operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="8e4ef-110">无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-110">Resource operations cannot be modified for built-in roles.This defines an operation or action that can be performed on an Intune resource (or entity).</span></span>  <span data-ttu-id="8e4ef-111">常用操作有获取、列出、删除、更新或创建。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-111">Common operations are Get, List, Delete, Update or Create.</span></span>  <span data-ttu-id="8e4ef-112">这些操作提供对基础 Intune 资源本身的基本管理。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-112">These operations provide basic management of the underlying Intune resource itself.</span></span>  <span data-ttu-id="8e4ef-113">某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-113">In some cases, an Intune resource can have operations that are used by the resource to take action in combination with other resources.</span></span>  <span data-ttu-id="8e4ef-114">例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-114">For example, the "Assign" operation is used to assign a MobileApp resource to an AAD security group.</span></span>  <span data-ttu-id="8e4ef-115">无法修改内置角色的资源操作。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-115">Resource operations cannot be modified for built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="8e4ef-116">方法</span><span class="sxs-lookup"><span data-stu-id="8e4ef-116">Methods</span></span>
|<span data-ttu-id="8e4ef-117">方法</span><span class="sxs-lookup"><span data-stu-id="8e4ef-117">Method</span></span>|<span data-ttu-id="8e4ef-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="8e4ef-118">Return Type</span></span>|<span data-ttu-id="8e4ef-119">说明</span><span class="sxs-lookup"><span data-stu-id="8e4ef-119">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e4ef-120">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="8e4ef-120">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="8e4ef-121">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e4ef-121">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="8e4ef-122">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-122">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="8e4ef-123">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-123">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="8e4ef-124">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-124">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="8e4ef-125">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-125">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="8e4ef-126">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-126">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="8e4ef-127">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-127">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="8e4ef-128">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-128">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="8e4ef-129">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-129">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="8e4ef-130">无</span><span class="sxs-lookup"><span data-stu-id="8e4ef-130">None</span></span>|<span data-ttu-id="8e4ef-131">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-131">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="8e4ef-132">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-132">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="8e4ef-133">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8e4ef-133">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="8e4ef-134">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-134">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e4ef-135">属性</span><span class="sxs-lookup"><span data-stu-id="8e4ef-135">Properties</span></span>
|<span data-ttu-id="8e4ef-136">属性</span><span class="sxs-lookup"><span data-stu-id="8e4ef-136">Property</span></span>|<span data-ttu-id="8e4ef-137">类型</span><span class="sxs-lookup"><span data-stu-id="8e4ef-137">Type</span></span>|<span data-ttu-id="8e4ef-138">说明</span><span class="sxs-lookup"><span data-stu-id="8e4ef-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e4ef-139">id</span><span class="sxs-lookup"><span data-stu-id="8e4ef-139">id</span></span>|<span data-ttu-id="8e4ef-140">字符串</span><span class="sxs-lookup"><span data-stu-id="8e4ef-140">String</span></span>|<span data-ttu-id="8e4ef-141">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-141">Key of the Resource Operation.</span></span> <span data-ttu-id="8e4ef-142">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-142">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="8e4ef-143">resourceName</span><span class="sxs-lookup"><span data-stu-id="8e4ef-143">resourceName</span></span>|<span data-ttu-id="8e4ef-144">String</span><span class="sxs-lookup"><span data-stu-id="8e4ef-144">String</span></span>|<span data-ttu-id="8e4ef-145">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-145">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="8e4ef-146">actionName</span><span class="sxs-lookup"><span data-stu-id="8e4ef-146">actionName</span></span>|<span data-ttu-id="8e4ef-147">String</span><span class="sxs-lookup"><span data-stu-id="8e4ef-147">String</span></span>|<span data-ttu-id="8e4ef-148">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-148">Type of action this operation is going to perform.</span></span> <span data-ttu-id="8e4ef-149">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-149">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="8e4ef-150">说明</span><span class="sxs-lookup"><span data-stu-id="8e4ef-150">description</span></span>|<span data-ttu-id="8e4ef-151">String</span><span class="sxs-lookup"><span data-stu-id="8e4ef-151">String</span></span>|<span data-ttu-id="8e4ef-152">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-152">Description of the resource operation.</span></span> <span data-ttu-id="8e4ef-153">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-153">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e4ef-154">关系</span><span class="sxs-lookup"><span data-stu-id="8e4ef-154">Relationships</span></span>
<span data-ttu-id="8e4ef-155">无</span><span class="sxs-lookup"><span data-stu-id="8e4ef-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e4ef-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e4ef-156">JSON Representation</span></span>
<span data-ttu-id="8e4ef-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e4ef-157">Here is a JSON representation of the resource.</span></span>
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



