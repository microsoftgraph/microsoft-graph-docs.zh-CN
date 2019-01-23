---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb72c4bf8cf7f2a4a55790087c3d46746c46a84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424656"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="86401-103">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="86401-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="86401-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="86401-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86401-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86401-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86401-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86401-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86401-107">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="86401-107">Represents an operation applied against an app registration.</span></span>

## <a name="methods"></a><span data-ttu-id="86401-108">方法</span><span class="sxs-lookup"><span data-stu-id="86401-108">Methods</span></span>
|<span data-ttu-id="86401-109">方法</span><span class="sxs-lookup"><span data-stu-id="86401-109">Method</span></span>|<span data-ttu-id="86401-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="86401-110">Return Type</span></span>|<span data-ttu-id="86401-111">说明</span><span class="sxs-lookup"><span data-stu-id="86401-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86401-112">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="86401-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="86401-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86401-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="86401-114">列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86401-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="86401-115">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="86401-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="86401-117">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86401-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="86401-118">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="86401-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="86401-120">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86401-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="86401-121">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="86401-122">无</span><span class="sxs-lookup"><span data-stu-id="86401-122">None</span></span>|<span data-ttu-id="86401-123">删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="86401-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="86401-124">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="86401-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="86401-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="86401-126">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86401-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86401-127">属性</span><span class="sxs-lookup"><span data-stu-id="86401-127">Properties</span></span>
|<span data-ttu-id="86401-128">属性</span><span class="sxs-lookup"><span data-stu-id="86401-128">Property</span></span>|<span data-ttu-id="86401-129">类型</span><span class="sxs-lookup"><span data-stu-id="86401-129">Type</span></span>|<span data-ttu-id="86401-130">说明</span><span class="sxs-lookup"><span data-stu-id="86401-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86401-131">displayName</span><span class="sxs-lookup"><span data-stu-id="86401-131">displayName</span></span>|<span data-ttu-id="86401-132">String</span><span class="sxs-lookup"><span data-stu-id="86401-132">String</span></span>|<span data-ttu-id="86401-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="86401-133">The operation name.</span></span>|
|<span data-ttu-id="86401-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86401-134">lastModifiedDateTime</span></span>|<span data-ttu-id="86401-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86401-135">DateTimeOffset</span></span>|<span data-ttu-id="86401-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="86401-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="86401-137">state</span><span class="sxs-lookup"><span data-stu-id="86401-137">state</span></span>|<span data-ttu-id="86401-138">String</span><span class="sxs-lookup"><span data-stu-id="86401-138">String</span></span>|<span data-ttu-id="86401-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="86401-139">The current state of the operation</span></span>|
|<span data-ttu-id="86401-140">id</span><span class="sxs-lookup"><span data-stu-id="86401-140">id</span></span>|<span data-ttu-id="86401-141">String</span><span class="sxs-lookup"><span data-stu-id="86401-141">String</span></span>|<span data-ttu-id="86401-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86401-142">Key of the entity.</span></span>|
|<span data-ttu-id="86401-143">version</span><span class="sxs-lookup"><span data-stu-id="86401-143">version</span></span>|<span data-ttu-id="86401-144">String</span><span class="sxs-lookup"><span data-stu-id="86401-144">String</span></span>|<span data-ttu-id="86401-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="86401-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86401-146">关系</span><span class="sxs-lookup"><span data-stu-id="86401-146">Relationships</span></span>
<span data-ttu-id="86401-147">无</span><span class="sxs-lookup"><span data-stu-id="86401-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86401-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86401-148">JSON Representation</span></span>
<span data-ttu-id="86401-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86401-149">Here is a JSON representation of the resource.</span></span>
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




