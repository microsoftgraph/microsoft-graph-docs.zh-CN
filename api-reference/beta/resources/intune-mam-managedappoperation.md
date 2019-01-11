---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 962468c4d1464b827e234b0aac5452bbd0be576a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859036"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="73d58-103">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="73d58-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="73d58-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73d58-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73d58-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73d58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73d58-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73d58-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73d58-107">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="73d58-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="73d58-108">方法</span><span class="sxs-lookup"><span data-stu-id="73d58-108">Methods</span></span>
|<span data-ttu-id="73d58-109">方法</span><span class="sxs-lookup"><span data-stu-id="73d58-109">Method</span></span>|<span data-ttu-id="73d58-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="73d58-110">Return Type</span></span>|<span data-ttu-id="73d58-111">说明</span><span class="sxs-lookup"><span data-stu-id="73d58-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73d58-112">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="73d58-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="73d58-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73d58-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="73d58-114">列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73d58-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="73d58-115">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="73d58-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="73d58-117">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73d58-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="73d58-118">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="73d58-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="73d58-120">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73d58-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="73d58-121">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="73d58-122">无</span><span class="sxs-lookup"><span data-stu-id="73d58-122">None</span></span>|<span data-ttu-id="73d58-123">删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="73d58-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="73d58-124">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="73d58-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="73d58-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="73d58-126">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73d58-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73d58-127">属性</span><span class="sxs-lookup"><span data-stu-id="73d58-127">Properties</span></span>
|<span data-ttu-id="73d58-128">属性</span><span class="sxs-lookup"><span data-stu-id="73d58-128">Property</span></span>|<span data-ttu-id="73d58-129">类型</span><span class="sxs-lookup"><span data-stu-id="73d58-129">Type</span></span>|<span data-ttu-id="73d58-130">说明</span><span class="sxs-lookup"><span data-stu-id="73d58-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73d58-131">displayName</span><span class="sxs-lookup"><span data-stu-id="73d58-131">displayName</span></span>|<span data-ttu-id="73d58-132">String</span><span class="sxs-lookup"><span data-stu-id="73d58-132">String</span></span>|<span data-ttu-id="73d58-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="73d58-133">The operation name.</span></span>|
|<span data-ttu-id="73d58-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73d58-134">lastModifiedDateTime</span></span>|<span data-ttu-id="73d58-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73d58-135">DateTimeOffset</span></span>|<span data-ttu-id="73d58-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="73d58-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="73d58-137">state</span><span class="sxs-lookup"><span data-stu-id="73d58-137">state</span></span>|<span data-ttu-id="73d58-138">String</span><span class="sxs-lookup"><span data-stu-id="73d58-138">String</span></span>|<span data-ttu-id="73d58-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="73d58-139">The current state of the operation</span></span>|
|<span data-ttu-id="73d58-140">id</span><span class="sxs-lookup"><span data-stu-id="73d58-140">id</span></span>|<span data-ttu-id="73d58-141">String</span><span class="sxs-lookup"><span data-stu-id="73d58-141">String</span></span>|<span data-ttu-id="73d58-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73d58-142">Key of the entity.</span></span>|
|<span data-ttu-id="73d58-143">version</span><span class="sxs-lookup"><span data-stu-id="73d58-143">version</span></span>|<span data-ttu-id="73d58-144">String</span><span class="sxs-lookup"><span data-stu-id="73d58-144">String</span></span>|<span data-ttu-id="73d58-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="73d58-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73d58-146">关系</span><span class="sxs-lookup"><span data-stu-id="73d58-146">Relationships</span></span>
<span data-ttu-id="73d58-147">无</span><span class="sxs-lookup"><span data-stu-id="73d58-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73d58-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73d58-148">JSON Representation</span></span>
<span data-ttu-id="73d58-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73d58-149">Here is a JSON representation of the resource.</span></span>
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





