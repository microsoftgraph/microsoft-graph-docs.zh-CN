---
title: resourceOperation 资源类型
description: 介绍 Microsoft Graph API (REST) 的 resourceOperation (实体) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d7e66c7cdbf7431d640d676c20bc074670cbd0a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751564"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="7a219-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a219-103">resourceOperation resource type</span></span>

<span data-ttu-id="7a219-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a219-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a219-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a219-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a219-106">介绍 Microsoft Graph API (REST) 的 resourceOperation (实体) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="7a219-106">Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).</span></span>

## <a name="methods"></a><span data-ttu-id="7a219-107">Methods</span><span class="sxs-lookup"><span data-stu-id="7a219-107">Methods</span></span>
|<span data-ttu-id="7a219-108">方法</span><span class="sxs-lookup"><span data-stu-id="7a219-108">Method</span></span>|<span data-ttu-id="7a219-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a219-109">Return Type</span></span>|<span data-ttu-id="7a219-110">Description</span><span class="sxs-lookup"><span data-stu-id="7a219-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a219-111">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="7a219-111">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="7a219-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7a219-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="7a219-113">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a219-113">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="7a219-114">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-114">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="7a219-115">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-115">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="7a219-116">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a219-116">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="7a219-117">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-117">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="7a219-118">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-118">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="7a219-119">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a219-119">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="7a219-120">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-120">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="7a219-121">无</span><span class="sxs-lookup"><span data-stu-id="7a219-121">None</span></span>|<span data-ttu-id="7a219-122">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="7a219-122">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="7a219-123">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-123">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="7a219-124">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7a219-124">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="7a219-125">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7a219-125">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a219-126">属性</span><span class="sxs-lookup"><span data-stu-id="7a219-126">Properties</span></span>
|<span data-ttu-id="7a219-127">属性</span><span class="sxs-lookup"><span data-stu-id="7a219-127">Property</span></span>|<span data-ttu-id="7a219-128">类型</span><span class="sxs-lookup"><span data-stu-id="7a219-128">Type</span></span>|<span data-ttu-id="7a219-129">说明</span><span class="sxs-lookup"><span data-stu-id="7a219-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a219-130">id</span><span class="sxs-lookup"><span data-stu-id="7a219-130">id</span></span>|<span data-ttu-id="7a219-131">String</span><span class="sxs-lookup"><span data-stu-id="7a219-131">String</span></span>|<span data-ttu-id="7a219-132">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="7a219-132">Key of the Resource Operation.</span></span> <span data-ttu-id="7a219-133">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="7a219-133">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="7a219-134">resourceName</span><span class="sxs-lookup"><span data-stu-id="7a219-134">resourceName</span></span>|<span data-ttu-id="7a219-135">String</span><span class="sxs-lookup"><span data-stu-id="7a219-135">String</span></span>|<span data-ttu-id="7a219-136">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="7a219-136">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="7a219-137">actionName</span><span class="sxs-lookup"><span data-stu-id="7a219-137">actionName</span></span>|<span data-ttu-id="7a219-138">String</span><span class="sxs-lookup"><span data-stu-id="7a219-138">String</span></span>|<span data-ttu-id="7a219-139">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="7a219-139">Type of action this operation is going to perform.</span></span> <span data-ttu-id="7a219-140">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="7a219-140">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="7a219-141">说明</span><span class="sxs-lookup"><span data-stu-id="7a219-141">description</span></span>|<span data-ttu-id="7a219-142">String</span><span class="sxs-lookup"><span data-stu-id="7a219-142">String</span></span>|<span data-ttu-id="7a219-143">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="7a219-143">Description of the resource operation.</span></span> <span data-ttu-id="7a219-144">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="7a219-144">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a219-145">关系</span><span class="sxs-lookup"><span data-stu-id="7a219-145">Relationships</span></span>
<span data-ttu-id="7a219-146">无</span><span class="sxs-lookup"><span data-stu-id="7a219-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a219-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a219-147">JSON Representation</span></span>
<span data-ttu-id="7a219-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a219-148">Here is a JSON representation of the resource.</span></span>
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




