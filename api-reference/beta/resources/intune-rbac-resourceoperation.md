---
title: resourceOperation 资源类型
description: 描述 resourceOperation 资源 (entity) of Microsoft Graph API (REST) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d19adde9ab960db3671a535169439640fa2a17f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039564"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="ff0d8-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff0d8-103">resourceOperation resource type</span></span>

<span data-ttu-id="ff0d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff0d8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff0d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff0d8-107">描述 resourceOperation 资源 (entity) of Microsoft Graph API (REST) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-107">Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).</span></span>

## <a name="methods"></a><span data-ttu-id="ff0d8-108">方法</span><span class="sxs-lookup"><span data-stu-id="ff0d8-108">Methods</span></span>
|<span data-ttu-id="ff0d8-109">方法</span><span class="sxs-lookup"><span data-stu-id="ff0d8-109">Method</span></span>|<span data-ttu-id="ff0d8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff0d8-110">Return Type</span></span>|<span data-ttu-id="ff0d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff0d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff0d8-112">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="ff0d8-112">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="ff0d8-113">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff0d8-113">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="ff0d8-114">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-114">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="ff0d8-115">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-115">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="ff0d8-116">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-116">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ff0d8-117">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-117">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ff0d8-118">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-118">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="ff0d8-119">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-119">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ff0d8-120">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-120">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ff0d8-121">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-121">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="ff0d8-122">无</span><span class="sxs-lookup"><span data-stu-id="ff0d8-122">None</span></span>|<span data-ttu-id="ff0d8-123">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-123">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="ff0d8-124">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-124">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="ff0d8-125">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-125">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="ff0d8-126">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-126">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="ff0d8-127">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="ff0d8-127">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="ff0d8-128">String collection</span><span class="sxs-lookup"><span data-stu-id="ff0d8-128">String collection</span></span>|<span data-ttu-id="ff0d8-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff0d8-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ff0d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff0d8-130">Properties</span></span>
|<span data-ttu-id="ff0d8-131">属性</span><span class="sxs-lookup"><span data-stu-id="ff0d8-131">Property</span></span>|<span data-ttu-id="ff0d8-132">类型</span><span class="sxs-lookup"><span data-stu-id="ff0d8-132">Type</span></span>|<span data-ttu-id="ff0d8-133">说明</span><span class="sxs-lookup"><span data-stu-id="ff0d8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0d8-134">id</span><span class="sxs-lookup"><span data-stu-id="ff0d8-134">id</span></span>|<span data-ttu-id="ff0d8-135">String</span><span class="sxs-lookup"><span data-stu-id="ff0d8-135">String</span></span>|<span data-ttu-id="ff0d8-136">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-136">Key of the Resource Operation.</span></span> <span data-ttu-id="ff0d8-137">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-137">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="ff0d8-138">resource</span><span class="sxs-lookup"><span data-stu-id="ff0d8-138">resource</span></span>|<span data-ttu-id="ff0d8-139">String</span><span class="sxs-lookup"><span data-stu-id="ff0d8-139">String</span></span>|<span data-ttu-id="ff0d8-140">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-140">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="ff0d8-141">resourceName</span><span class="sxs-lookup"><span data-stu-id="ff0d8-141">resourceName</span></span>|<span data-ttu-id="ff0d8-142">String</span><span class="sxs-lookup"><span data-stu-id="ff0d8-142">String</span></span>|<span data-ttu-id="ff0d8-143">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-143">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="ff0d8-144">actionName</span><span class="sxs-lookup"><span data-stu-id="ff0d8-144">actionName</span></span>|<span data-ttu-id="ff0d8-145">String</span><span class="sxs-lookup"><span data-stu-id="ff0d8-145">String</span></span>|<span data-ttu-id="ff0d8-146">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-146">Type of action this operation is going to perform.</span></span> <span data-ttu-id="ff0d8-147">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-147">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="ff0d8-148">description</span><span class="sxs-lookup"><span data-stu-id="ff0d8-148">description</span></span>|<span data-ttu-id="ff0d8-149">String</span><span class="sxs-lookup"><span data-stu-id="ff0d8-149">String</span></span>|<span data-ttu-id="ff0d8-150">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-150">Description of the resource operation.</span></span> <span data-ttu-id="ff0d8-151">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-151">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="ff0d8-152">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="ff0d8-152">enabledForScopeValidation</span></span>|<span data-ttu-id="ff0d8-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff0d8-153">Boolean</span></span>|<span data-ttu-id="ff0d8-154">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-154">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff0d8-155">关系</span><span class="sxs-lookup"><span data-stu-id="ff0d8-155">Relationships</span></span>
<span data-ttu-id="ff0d8-156">无</span><span class="sxs-lookup"><span data-stu-id="ff0d8-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff0d8-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff0d8-157">JSON Representation</span></span>
<span data-ttu-id="ff0d8-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff0d8-158">Here is a JSON representation of the resource.</span></span>
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






