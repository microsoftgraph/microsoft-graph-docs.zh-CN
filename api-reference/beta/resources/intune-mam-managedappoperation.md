---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5ad689737da4944f973c813615ddc2b0cb2f8c1f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302640"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="23d40-103">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="23d40-103">managedAppOperation resource type</span></span>

<span data-ttu-id="23d40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23d40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23d40-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23d40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23d40-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23d40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23d40-107">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="23d40-107">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="23d40-108">Methods</span><span class="sxs-lookup"><span data-stu-id="23d40-108">Methods</span></span>
|<span data-ttu-id="23d40-109">方法</span><span class="sxs-lookup"><span data-stu-id="23d40-109">Method</span></span>|<span data-ttu-id="23d40-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="23d40-110">Return Type</span></span>|<span data-ttu-id="23d40-111">Description</span><span class="sxs-lookup"><span data-stu-id="23d40-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23d40-112">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="23d40-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="23d40-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23d40-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="23d40-114">列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23d40-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="23d40-115">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="23d40-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="23d40-117">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23d40-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="23d40-118">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="23d40-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="23d40-120">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23d40-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="23d40-121">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="23d40-122">无</span><span class="sxs-lookup"><span data-stu-id="23d40-122">None</span></span>|<span data-ttu-id="23d40-123">删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="23d40-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="23d40-124">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="23d40-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="23d40-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="23d40-126">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23d40-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23d40-127">属性</span><span class="sxs-lookup"><span data-stu-id="23d40-127">Properties</span></span>
|<span data-ttu-id="23d40-128">属性</span><span class="sxs-lookup"><span data-stu-id="23d40-128">Property</span></span>|<span data-ttu-id="23d40-129">类型</span><span class="sxs-lookup"><span data-stu-id="23d40-129">Type</span></span>|<span data-ttu-id="23d40-130">说明</span><span class="sxs-lookup"><span data-stu-id="23d40-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23d40-131">displayName</span><span class="sxs-lookup"><span data-stu-id="23d40-131">displayName</span></span>|<span data-ttu-id="23d40-132">字符串</span><span class="sxs-lookup"><span data-stu-id="23d40-132">String</span></span>|<span data-ttu-id="23d40-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="23d40-133">The operation name.</span></span>|
|<span data-ttu-id="23d40-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23d40-134">lastModifiedDateTime</span></span>|<span data-ttu-id="23d40-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23d40-135">DateTimeOffset</span></span>|<span data-ttu-id="23d40-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="23d40-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="23d40-137">state</span><span class="sxs-lookup"><span data-stu-id="23d40-137">state</span></span>|<span data-ttu-id="23d40-138">String</span><span class="sxs-lookup"><span data-stu-id="23d40-138">String</span></span>|<span data-ttu-id="23d40-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="23d40-139">The current state of the operation</span></span>|
|<span data-ttu-id="23d40-140">id</span><span class="sxs-lookup"><span data-stu-id="23d40-140">id</span></span>|<span data-ttu-id="23d40-141">字符串</span><span class="sxs-lookup"><span data-stu-id="23d40-141">String</span></span>|<span data-ttu-id="23d40-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="23d40-142">Key of the entity.</span></span>|
|<span data-ttu-id="23d40-143">version</span><span class="sxs-lookup"><span data-stu-id="23d40-143">version</span></span>|<span data-ttu-id="23d40-144">String</span><span class="sxs-lookup"><span data-stu-id="23d40-144">String</span></span>|<span data-ttu-id="23d40-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="23d40-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23d40-146">关系</span><span class="sxs-lookup"><span data-stu-id="23d40-146">Relationships</span></span>
<span data-ttu-id="23d40-147">无</span><span class="sxs-lookup"><span data-stu-id="23d40-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23d40-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23d40-148">JSON Representation</span></span>
<span data-ttu-id="23d40-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23d40-149">Here is a JSON representation of the resource.</span></span>
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




