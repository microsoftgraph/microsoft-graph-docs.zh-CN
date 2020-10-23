---
title: resourceOperation 资源类型
description: 描述 resourceOperation 资源 (entity) of Microsoft Graph API (REST) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4aac5d65bc0f743671cdea979fca286d6023aa8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728051"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="1a5ae-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a5ae-103">resourceOperation resource type</span></span>

<span data-ttu-id="1a5ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a5ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a5ae-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a5ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a5ae-107">描述 resourceOperation 资源 (entity) of Microsoft Graph API (REST) ，它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-107">Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).</span></span>

## <a name="methods"></a><span data-ttu-id="1a5ae-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1a5ae-108">Methods</span></span>
|<span data-ttu-id="1a5ae-109">方法</span><span class="sxs-lookup"><span data-stu-id="1a5ae-109">Method</span></span>|<span data-ttu-id="1a5ae-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a5ae-110">Return Type</span></span>|<span data-ttu-id="1a5ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a5ae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a5ae-112">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="1a5ae-112">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="1a5ae-113">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a5ae-113">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="1a5ae-114">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-114">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="1a5ae-115">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-115">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="1a5ae-116">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-116">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="1a5ae-117">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-117">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="1a5ae-118">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-118">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="1a5ae-119">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-119">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="1a5ae-120">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-120">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="1a5ae-121">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-121">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="1a5ae-122">无</span><span class="sxs-lookup"><span data-stu-id="1a5ae-122">None</span></span>|<span data-ttu-id="1a5ae-123">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-123">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="1a5ae-124">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-124">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="1a5ae-125">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-125">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="1a5ae-126">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-126">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="1a5ae-127">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="1a5ae-127">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="1a5ae-128">String collection</span><span class="sxs-lookup"><span data-stu-id="1a5ae-128">String collection</span></span>|<span data-ttu-id="1a5ae-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1a5ae-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1a5ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a5ae-130">Properties</span></span>
|<span data-ttu-id="1a5ae-131">属性</span><span class="sxs-lookup"><span data-stu-id="1a5ae-131">Property</span></span>|<span data-ttu-id="1a5ae-132">类型</span><span class="sxs-lookup"><span data-stu-id="1a5ae-132">Type</span></span>|<span data-ttu-id="1a5ae-133">说明</span><span class="sxs-lookup"><span data-stu-id="1a5ae-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a5ae-134">id</span><span class="sxs-lookup"><span data-stu-id="1a5ae-134">id</span></span>|<span data-ttu-id="1a5ae-135">String</span><span class="sxs-lookup"><span data-stu-id="1a5ae-135">String</span></span>|<span data-ttu-id="1a5ae-136">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-136">Key of the Resource Operation.</span></span> <span data-ttu-id="1a5ae-137">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-137">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="1a5ae-138">resource</span><span class="sxs-lookup"><span data-stu-id="1a5ae-138">resource</span></span>|<span data-ttu-id="1a5ae-139">String</span><span class="sxs-lookup"><span data-stu-id="1a5ae-139">String</span></span>|<span data-ttu-id="1a5ae-140">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-140">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="1a5ae-141">resourceName</span><span class="sxs-lookup"><span data-stu-id="1a5ae-141">resourceName</span></span>|<span data-ttu-id="1a5ae-142">String</span><span class="sxs-lookup"><span data-stu-id="1a5ae-142">String</span></span>|<span data-ttu-id="1a5ae-143">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-143">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="1a5ae-144">actionName</span><span class="sxs-lookup"><span data-stu-id="1a5ae-144">actionName</span></span>|<span data-ttu-id="1a5ae-145">String</span><span class="sxs-lookup"><span data-stu-id="1a5ae-145">String</span></span>|<span data-ttu-id="1a5ae-146">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-146">Type of action this operation is going to perform.</span></span> <span data-ttu-id="1a5ae-147">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-147">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="1a5ae-148">说明</span><span class="sxs-lookup"><span data-stu-id="1a5ae-148">description</span></span>|<span data-ttu-id="1a5ae-149">String</span><span class="sxs-lookup"><span data-stu-id="1a5ae-149">String</span></span>|<span data-ttu-id="1a5ae-150">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-150">Description of the resource operation.</span></span> <span data-ttu-id="1a5ae-151">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-151">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="1a5ae-152">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="1a5ae-152">enabledForScopeValidation</span></span>|<span data-ttu-id="1a5ae-153">布尔</span><span class="sxs-lookup"><span data-stu-id="1a5ae-153">Boolean</span></span>|<span data-ttu-id="1a5ae-154">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-154">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a5ae-155">关系</span><span class="sxs-lookup"><span data-stu-id="1a5ae-155">Relationships</span></span>
<span data-ttu-id="1a5ae-156">无</span><span class="sxs-lookup"><span data-stu-id="1a5ae-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a5ae-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a5ae-157">JSON Representation</span></span>
<span data-ttu-id="1a5ae-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a5ae-158">Here is a JSON representation of the resource.</span></span>
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





