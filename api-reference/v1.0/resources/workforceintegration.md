---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 715c78e8cb412f11b7b336680e3c433369c9e608
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015097"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="35d81-103">workforceIntegration 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d81-103">workforceIntegration resource type</span></span>

<span data-ttu-id="35d81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35d81-105">员工的一个实例与倒班的集成。</span><span class="sxs-lookup"><span data-stu-id="35d81-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="35d81-106">方法</span><span class="sxs-lookup"><span data-stu-id="35d81-106">Methods</span></span>

| <span data-ttu-id="35d81-107">方法</span><span class="sxs-lookup"><span data-stu-id="35d81-107">Method</span></span>       | <span data-ttu-id="35d81-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="35d81-108">Return Type</span></span> | <span data-ttu-id="35d81-109">说明</span><span class="sxs-lookup"><span data-stu-id="35d81-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="35d81-110">创建</span><span class="sxs-lookup"><span data-stu-id="35d81-110">Create</span></span>](../api/workforceintegration-post.md) | [<span data-ttu-id="35d81-111">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="35d81-111">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="35d81-112">创建新的 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="35d81-112">Create a new **workforceIntegration** object.</span></span>|
| [<span data-ttu-id="35d81-113">List</span><span class="sxs-lookup"><span data-stu-id="35d81-113">List</span></span>](../api/workforceintegration-list.md) | <span data-ttu-id="35d81-114">[workforceIntegration](workforceintegration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35d81-114">[workforceIntegration](workforceintegration.md) collection</span></span> | <span data-ttu-id="35d81-115">获取与此计划关联的 **workforceIntegration** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="35d81-115">Get the list of **workforceIntegration** objects associated with this schedule.</span></span>|
| [<span data-ttu-id="35d81-116">获取</span><span class="sxs-lookup"><span data-stu-id="35d81-116">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="35d81-117">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="35d81-117">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="35d81-118">读取 **workforceIntegration** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35d81-118">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="35d81-119">更新</span><span class="sxs-lookup"><span data-stu-id="35d81-119">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="35d81-120">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="35d81-120">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="35d81-121">更新 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="35d81-121">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="35d81-122">删除</span><span class="sxs-lookup"><span data-stu-id="35d81-122">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="35d81-123">无</span><span class="sxs-lookup"><span data-stu-id="35d81-123">None</span></span> | <span data-ttu-id="35d81-124">删除 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="35d81-124">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35d81-125">属性</span><span class="sxs-lookup"><span data-stu-id="35d81-125">Properties</span></span>

| <span data-ttu-id="35d81-126">属性</span><span class="sxs-lookup"><span data-stu-id="35d81-126">Property</span></span>     | <span data-ttu-id="35d81-127">类型</span><span class="sxs-lookup"><span data-stu-id="35d81-127">Type</span></span>        | <span data-ttu-id="35d81-128">说明</span><span class="sxs-lookup"><span data-stu-id="35d81-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="35d81-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="35d81-129">apiVersion</span></span>|<span data-ttu-id="35d81-130">Int32</span><span class="sxs-lookup"><span data-stu-id="35d81-130">Int32</span></span>|<span data-ttu-id="35d81-131">回调 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="35d81-131">API version for the call back URL.</span></span> <span data-ttu-id="35d81-132">从1开始。</span><span class="sxs-lookup"><span data-stu-id="35d81-132">Start with 1.</span></span>|
|<span data-ttu-id="35d81-133">displayName</span><span class="sxs-lookup"><span data-stu-id="35d81-133">displayName</span></span>|<span data-ttu-id="35d81-134">String</span><span class="sxs-lookup"><span data-stu-id="35d81-134">String</span></span>|<span data-ttu-id="35d81-135">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="35d81-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="35d81-136">技术</span><span class="sxs-lookup"><span data-stu-id="35d81-136">encryption</span></span>|[<span data-ttu-id="35d81-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="35d81-137">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="35d81-138">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="35d81-138">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="35d81-139">isActive</span><span class="sxs-lookup"><span data-stu-id="35d81-139">isActive</span></span>|<span data-ttu-id="35d81-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="35d81-140">Boolean</span></span>|<span data-ttu-id="35d81-141">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="35d81-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="35d81-142">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="35d81-142">supportedEntities</span></span>|<span data-ttu-id="35d81-143">字符串</span><span class="sxs-lookup"><span data-stu-id="35d81-143">string</span></span>| <span data-ttu-id="35d81-144">移位支持同步更改通知的实体。</span><span class="sxs-lookup"><span data-stu-id="35d81-144">The Shifts entities supported for synchronous change notifications.</span></span> <span data-ttu-id="35d81-145">班次将回拨到在此处添加的这些实体上的客户端更改上提供的 url。</span><span class="sxs-lookup"><span data-stu-id="35d81-145">Shifts will make a call back to the url provided on client changes on those entities added here.</span></span> <span data-ttu-id="35d81-146">默认情况下，不支持更改通知的任何实体。</span><span class="sxs-lookup"><span data-stu-id="35d81-146">By default, no entities are supported for change notifications.</span></span> <span data-ttu-id="35d81-147">可能的值为 `none` ： `shift` 、 `swapRequest` 、 `openshift` `openShiftRequest` 、、 `userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="35d81-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="35d81-148">url</span><span class="sxs-lookup"><span data-stu-id="35d81-148">url</span></span>|<span data-ttu-id="35d81-149">String</span><span class="sxs-lookup"><span data-stu-id="35d81-149">String</span></span>| <span data-ttu-id="35d81-150">来自倒班服务的回调的劳动力集成 URL。</span><span class="sxs-lookup"><span data-stu-id="35d81-150">Workforce Integration URL for callbacks from the Shifts service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d81-151">关系</span><span class="sxs-lookup"><span data-stu-id="35d81-151">Relationships</span></span>

<span data-ttu-id="35d81-152">无。</span><span class="sxs-lookup"><span data-stu-id="35d81-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d81-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d81-153">JSON representation</span></span>

<span data-ttu-id="35d81-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d81-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supportedEntities": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

