---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
ms.openlocfilehash: 267adafc5a74ad447dfb3468cf9238e1c4642e5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041547"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="071d2-103">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="071d2-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="071d2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="071d2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="071d2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="071d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="071d2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="071d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="071d2-107">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="071d2-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="071d2-108">方法</span><span class="sxs-lookup"><span data-stu-id="071d2-108">Methods</span></span>
|<span data-ttu-id="071d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="071d2-109">Method</span></span>|<span data-ttu-id="071d2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="071d2-110">Return Type</span></span>|<span data-ttu-id="071d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="071d2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="071d2-112">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="071d2-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="071d2-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="071d2-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="071d2-114">列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="071d2-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="071d2-115">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="071d2-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="071d2-117">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="071d2-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="071d2-118">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="071d2-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="071d2-120">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="071d2-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="071d2-121">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="071d2-122">无</span><span class="sxs-lookup"><span data-stu-id="071d2-122">None</span></span>|<span data-ttu-id="071d2-123">删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="071d2-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="071d2-124">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="071d2-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="071d2-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="071d2-126">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="071d2-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="071d2-127">属性</span><span class="sxs-lookup"><span data-stu-id="071d2-127">Properties</span></span>
|<span data-ttu-id="071d2-128">属性</span><span class="sxs-lookup"><span data-stu-id="071d2-128">Property</span></span>|<span data-ttu-id="071d2-129">类型</span><span class="sxs-lookup"><span data-stu-id="071d2-129">Type</span></span>|<span data-ttu-id="071d2-130">说明</span><span class="sxs-lookup"><span data-stu-id="071d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="071d2-131">displayName</span><span class="sxs-lookup"><span data-stu-id="071d2-131">displayName</span></span>|<span data-ttu-id="071d2-132">String</span><span class="sxs-lookup"><span data-stu-id="071d2-132">String</span></span>|<span data-ttu-id="071d2-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="071d2-133">The operation name.</span></span>|
|<span data-ttu-id="071d2-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="071d2-134">lastModifiedDateTime</span></span>|<span data-ttu-id="071d2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="071d2-135">DateTimeOffset</span></span>|<span data-ttu-id="071d2-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="071d2-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="071d2-137">state</span><span class="sxs-lookup"><span data-stu-id="071d2-137">state</span></span>|<span data-ttu-id="071d2-138">String</span><span class="sxs-lookup"><span data-stu-id="071d2-138">String</span></span>|<span data-ttu-id="071d2-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="071d2-139">The current state of the operation</span></span>|
|<span data-ttu-id="071d2-140">id</span><span class="sxs-lookup"><span data-stu-id="071d2-140">id</span></span>|<span data-ttu-id="071d2-141">String</span><span class="sxs-lookup"><span data-stu-id="071d2-141">String</span></span>|<span data-ttu-id="071d2-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="071d2-142">Key of the entity.</span></span>|
|<span data-ttu-id="071d2-143">version</span><span class="sxs-lookup"><span data-stu-id="071d2-143">version</span></span>|<span data-ttu-id="071d2-144">String</span><span class="sxs-lookup"><span data-stu-id="071d2-144">String</span></span>|<span data-ttu-id="071d2-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="071d2-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="071d2-146">关系</span><span class="sxs-lookup"><span data-stu-id="071d2-146">Relationships</span></span>
<span data-ttu-id="071d2-147">无</span><span class="sxs-lookup"><span data-stu-id="071d2-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="071d2-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="071d2-148">JSON Representation</span></span>
<span data-ttu-id="071d2-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="071d2-149">Here is a JSON representation of the resource.</span></span>
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





