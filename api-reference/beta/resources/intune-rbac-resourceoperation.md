---
title: resourceOperation 资源类型
description: 介绍 Microsoft Graph API (REST) 的 resourceOperation 资源 (实体), 它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b83ad1c902e8455d42ae0e9805bf6881b49ef3b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369281"
---
# <a name="resourceoperation-resource-type"></a><span data-ttu-id="1fa59-103">resourceOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fa59-103">resourceOperation resource type</span></span>

> <span data-ttu-id="1fa59-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1fa59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fa59-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fa59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fa59-106">介绍 Microsoft Graph API (REST) 的 resourceOperation 资源 (实体), 它支持与基于角色的访问控制 (RBAC) 相关的 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="1fa59-106">Describes the resourceOperation resource (entity) of the Microsoft Graph API (REST), which supports Intune workflows related to role-based access control (RBAC).</span></span>

## <a name="methods"></a><span data-ttu-id="1fa59-107">方法</span><span class="sxs-lookup"><span data-stu-id="1fa59-107">Methods</span></span>
|<span data-ttu-id="1fa59-108">方法</span><span class="sxs-lookup"><span data-stu-id="1fa59-108">Method</span></span>|<span data-ttu-id="1fa59-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1fa59-109">Return Type</span></span>|<span data-ttu-id="1fa59-110">说明</span><span class="sxs-lookup"><span data-stu-id="1fa59-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fa59-111">List resourceOperations</span><span class="sxs-lookup"><span data-stu-id="1fa59-111">List resourceOperations</span></span>](../api/intune-rbac-resourceoperation-list.md)|<span data-ttu-id="1fa59-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fa59-112">[resourceOperation](../resources/intune-rbac-resourceoperation.md) collection</span></span>|<span data-ttu-id="1fa59-113">列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fa59-113">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>|
|[<span data-ttu-id="1fa59-114">Get resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-114">Get resourceOperation</span></span>](../api/intune-rbac-resourceoperation-get.md)|[<span data-ttu-id="1fa59-115">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-115">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="1fa59-116">读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fa59-116">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="1fa59-117">Create resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-117">Create resourceOperation</span></span>](../api/intune-rbac-resourceoperation-create.md)|[<span data-ttu-id="1fa59-118">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-118">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="1fa59-119">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fa59-119">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="1fa59-120">Delete resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-120">Delete resourceOperation</span></span>](../api/intune-rbac-resourceoperation-delete.md)|<span data-ttu-id="1fa59-121">无</span><span class="sxs-lookup"><span data-stu-id="1fa59-121">None</span></span>|<span data-ttu-id="1fa59-122">删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="1fa59-122">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>|
|[<span data-ttu-id="1fa59-123">Update resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-123">Update resourceOperation</span></span>](../api/intune-rbac-resourceoperation-update.md)|[<span data-ttu-id="1fa59-124">resourceOperation</span><span class="sxs-lookup"><span data-stu-id="1fa59-124">resourceOperation</span></span>](../resources/intune-rbac-resourceoperation.md)|<span data-ttu-id="1fa59-125">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1fa59-125">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>|
|[<span data-ttu-id="1fa59-126">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="1fa59-126">getScopesForUser function</span></span>](../api/intune-rbac-resourceoperation-getscopesforuser.md)|<span data-ttu-id="1fa59-127">String collection</span><span class="sxs-lookup"><span data-stu-id="1fa59-127">String collection</span></span>|<span data-ttu-id="1fa59-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1fa59-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1fa59-129">属性</span><span class="sxs-lookup"><span data-stu-id="1fa59-129">Properties</span></span>
|<span data-ttu-id="1fa59-130">属性</span><span class="sxs-lookup"><span data-stu-id="1fa59-130">Property</span></span>|<span data-ttu-id="1fa59-131">类型</span><span class="sxs-lookup"><span data-stu-id="1fa59-131">Type</span></span>|<span data-ttu-id="1fa59-132">说明</span><span class="sxs-lookup"><span data-stu-id="1fa59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa59-133">id</span><span class="sxs-lookup"><span data-stu-id="1fa59-133">id</span></span>|<span data-ttu-id="1fa59-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1fa59-134">String</span></span>|<span data-ttu-id="1fa59-135">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="1fa59-135">Key of the Resource Operation.</span></span> <span data-ttu-id="1fa59-136">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="1fa59-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="1fa59-137">resource</span><span class="sxs-lookup"><span data-stu-id="1fa59-137">resource</span></span>|<span data-ttu-id="1fa59-138">String</span><span class="sxs-lookup"><span data-stu-id="1fa59-138">String</span></span>|<span data-ttu-id="1fa59-139">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="1fa59-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="1fa59-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="1fa59-140">resourceName</span></span>|<span data-ttu-id="1fa59-141">String</span><span class="sxs-lookup"><span data-stu-id="1fa59-141">String</span></span>|<span data-ttu-id="1fa59-142">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="1fa59-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="1fa59-143">actionName</span><span class="sxs-lookup"><span data-stu-id="1fa59-143">actionName</span></span>|<span data-ttu-id="1fa59-144">String</span><span class="sxs-lookup"><span data-stu-id="1fa59-144">String</span></span>|<span data-ttu-id="1fa59-145">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="1fa59-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="1fa59-146">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="1fa59-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="1fa59-147">说明</span><span class="sxs-lookup"><span data-stu-id="1fa59-147">description</span></span>|<span data-ttu-id="1fa59-148">String</span><span class="sxs-lookup"><span data-stu-id="1fa59-148">String</span></span>|<span data-ttu-id="1fa59-149">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="1fa59-149">Description of the resource operation.</span></span> <span data-ttu-id="1fa59-150">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="1fa59-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="1fa59-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="1fa59-151">enabledForScopeValidation</span></span>|<span data-ttu-id="1fa59-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa59-152">Boolean</span></span>|<span data-ttu-id="1fa59-153">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="1fa59-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fa59-154">关系</span><span class="sxs-lookup"><span data-stu-id="1fa59-154">Relationships</span></span>
<span data-ttu-id="1fa59-155">无</span><span class="sxs-lookup"><span data-stu-id="1fa59-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fa59-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fa59-156">JSON Representation</span></span>
<span data-ttu-id="1fa59-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fa59-157">Here is a JSON representation of the resource.</span></span>
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



