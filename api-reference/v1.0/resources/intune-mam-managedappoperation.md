---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87b18c311c263dfb70c2aa8015044d280a48c6cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406620"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="b405e-103">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b405e-103">managedAppOperation resource type</span></span>

<span data-ttu-id="b405e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b405e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b405e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b405e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b405e-106">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="b405e-106">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="b405e-107">方法</span><span class="sxs-lookup"><span data-stu-id="b405e-107">Methods</span></span>
|<span data-ttu-id="b405e-108">方法</span><span class="sxs-lookup"><span data-stu-id="b405e-108">Method</span></span>|<span data-ttu-id="b405e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b405e-109">Return Type</span></span>|<span data-ttu-id="b405e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b405e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b405e-111">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="b405e-111">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="b405e-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b405e-112">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="b405e-113">列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b405e-113">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="b405e-114">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-114">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="b405e-115">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-115">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b405e-116">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b405e-116">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="b405e-117">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-117">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="b405e-118">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-118">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b405e-119">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b405e-119">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="b405e-120">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-120">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="b405e-121">无</span><span class="sxs-lookup"><span data-stu-id="b405e-121">None</span></span>|<span data-ttu-id="b405e-122">删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="b405e-122">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="b405e-123">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-123">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="b405e-124">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b405e-124">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b405e-125">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b405e-125">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b405e-126">属性</span><span class="sxs-lookup"><span data-stu-id="b405e-126">Properties</span></span>
|<span data-ttu-id="b405e-127">属性</span><span class="sxs-lookup"><span data-stu-id="b405e-127">Property</span></span>|<span data-ttu-id="b405e-128">类型</span><span class="sxs-lookup"><span data-stu-id="b405e-128">Type</span></span>|<span data-ttu-id="b405e-129">说明</span><span class="sxs-lookup"><span data-stu-id="b405e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b405e-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b405e-130">displayName</span></span>|<span data-ttu-id="b405e-131">String</span><span class="sxs-lookup"><span data-stu-id="b405e-131">String</span></span>|<span data-ttu-id="b405e-132">操作名称。</span><span class="sxs-lookup"><span data-stu-id="b405e-132">The operation name.</span></span>|
|<span data-ttu-id="b405e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b405e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b405e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b405e-134">DateTimeOffset</span></span>|<span data-ttu-id="b405e-135">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="b405e-135">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b405e-136">state</span><span class="sxs-lookup"><span data-stu-id="b405e-136">state</span></span>|<span data-ttu-id="b405e-137">String</span><span class="sxs-lookup"><span data-stu-id="b405e-137">String</span></span>|<span data-ttu-id="b405e-138">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="b405e-138">The current state of the operation</span></span>|
|<span data-ttu-id="b405e-139">id</span><span class="sxs-lookup"><span data-stu-id="b405e-139">id</span></span>|<span data-ttu-id="b405e-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b405e-140">String</span></span>|<span data-ttu-id="b405e-141">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b405e-141">Key of the entity.</span></span>|
|<span data-ttu-id="b405e-142">version</span><span class="sxs-lookup"><span data-stu-id="b405e-142">version</span></span>|<span data-ttu-id="b405e-143">String</span><span class="sxs-lookup"><span data-stu-id="b405e-143">String</span></span>|<span data-ttu-id="b405e-144">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b405e-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b405e-145">关系</span><span class="sxs-lookup"><span data-stu-id="b405e-145">Relationships</span></span>
<span data-ttu-id="b405e-146">无</span><span class="sxs-lookup"><span data-stu-id="b405e-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b405e-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b405e-147">JSON Representation</span></span>
<span data-ttu-id="b405e-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b405e-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```







