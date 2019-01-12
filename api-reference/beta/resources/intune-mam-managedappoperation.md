---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a8c7ee3f49ad9b98d680662834911c2d20984d8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951794"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="b1de4-103">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1de4-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="b1de4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1de4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1de4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1de4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1de4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b1de4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1de4-107">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="b1de4-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="b1de4-108">方法</span><span class="sxs-lookup"><span data-stu-id="b1de4-108">Methods</span></span>
|<span data-ttu-id="b1de4-109">方法</span><span class="sxs-lookup"><span data-stu-id="b1de4-109">Method</span></span>|<span data-ttu-id="b1de4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1de4-110">Return Type</span></span>|<span data-ttu-id="b1de4-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1de4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1de4-112">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="b1de4-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="b1de4-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1de4-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="b1de4-114">列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1de4-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="b1de4-115">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="b1de4-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b1de4-117">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1de4-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="b1de4-118">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="b1de4-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b1de4-120">创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1de4-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="b1de4-121">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="b1de4-122">无</span><span class="sxs-lookup"><span data-stu-id="b1de4-122">None</span></span>|<span data-ttu-id="b1de4-123">删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="b1de4-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="b1de4-124">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="b1de4-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b1de4-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="b1de4-126">更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1de4-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1de4-127">属性</span><span class="sxs-lookup"><span data-stu-id="b1de4-127">Properties</span></span>
|<span data-ttu-id="b1de4-128">属性</span><span class="sxs-lookup"><span data-stu-id="b1de4-128">Property</span></span>|<span data-ttu-id="b1de4-129">类型</span><span class="sxs-lookup"><span data-stu-id="b1de4-129">Type</span></span>|<span data-ttu-id="b1de4-130">说明</span><span class="sxs-lookup"><span data-stu-id="b1de4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1de4-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b1de4-131">displayName</span></span>|<span data-ttu-id="b1de4-132">String</span><span class="sxs-lookup"><span data-stu-id="b1de4-132">String</span></span>|<span data-ttu-id="b1de4-133">操作名称。</span><span class="sxs-lookup"><span data-stu-id="b1de4-133">The operation name.</span></span>|
|<span data-ttu-id="b1de4-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1de4-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b1de4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1de4-135">DateTimeOffset</span></span>|<span data-ttu-id="b1de4-136">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="b1de4-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b1de4-137">state</span><span class="sxs-lookup"><span data-stu-id="b1de4-137">state</span></span>|<span data-ttu-id="b1de4-138">String</span><span class="sxs-lookup"><span data-stu-id="b1de4-138">String</span></span>|<span data-ttu-id="b1de4-139">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="b1de4-139">The current state of the operation</span></span>|
|<span data-ttu-id="b1de4-140">id</span><span class="sxs-lookup"><span data-stu-id="b1de4-140">id</span></span>|<span data-ttu-id="b1de4-141">String</span><span class="sxs-lookup"><span data-stu-id="b1de4-141">String</span></span>|<span data-ttu-id="b1de4-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1de4-142">Key of the entity.</span></span>|
|<span data-ttu-id="b1de4-143">version</span><span class="sxs-lookup"><span data-stu-id="b1de4-143">version</span></span>|<span data-ttu-id="b1de4-144">String</span><span class="sxs-lookup"><span data-stu-id="b1de4-144">String</span></span>|<span data-ttu-id="b1de4-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b1de4-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1de4-146">关系</span><span class="sxs-lookup"><span data-stu-id="b1de4-146">Relationships</span></span>
<span data-ttu-id="b1de4-147">无</span><span class="sxs-lookup"><span data-stu-id="b1de4-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1de4-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1de4-148">JSON Representation</span></span>
<span data-ttu-id="b1de4-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1de4-149">Here is a JSON representation of the resource.</span></span>
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





