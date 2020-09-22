---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 93621d89df8e3bf4c3f95c1a89814af8899fc13d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019402"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="9df02-103">workforceIntegration 资源类型</span><span class="sxs-lookup"><span data-stu-id="9df02-103">workforceIntegration resource type</span></span>

<span data-ttu-id="9df02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df02-105">员工的一个实例与倒班的集成。</span><span class="sxs-lookup"><span data-stu-id="9df02-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="9df02-106">方法</span><span class="sxs-lookup"><span data-stu-id="9df02-106">Methods</span></span>

| <span data-ttu-id="9df02-107">方法</span><span class="sxs-lookup"><span data-stu-id="9df02-107">Method</span></span>       | <span data-ttu-id="9df02-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9df02-108">Return Type</span></span> | <span data-ttu-id="9df02-109">Description</span><span class="sxs-lookup"><span data-stu-id="9df02-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9df02-110">List</span><span class="sxs-lookup"><span data-stu-id="9df02-110">List</span></span>](../api/workforceintegration-list.md) | <span data-ttu-id="9df02-111">[workforceIntegration](workforceintegration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9df02-111">[workforceIntegration](workforceintegration.md) collection</span></span> | <span data-ttu-id="9df02-112">获取与此计划关联的 **workforceIntegration** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9df02-112">Get the list of **workforceIntegration** objects associated with this schedule.</span></span>|
| [<span data-ttu-id="9df02-113">创建</span><span class="sxs-lookup"><span data-stu-id="9df02-113">Create</span></span>](../api/workforceintegration-post.md) | [<span data-ttu-id="9df02-114">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="9df02-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="9df02-115">创建新的 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="9df02-115">Create a new **workforceIntegration** object.</span></span>|
| [<span data-ttu-id="9df02-116">获取</span><span class="sxs-lookup"><span data-stu-id="9df02-116">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="9df02-117">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="9df02-117">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="9df02-118">读取 **workforceIntegration** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9df02-118">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="9df02-119">更新</span><span class="sxs-lookup"><span data-stu-id="9df02-119">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="9df02-120">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="9df02-120">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="9df02-121">更新 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="9df02-121">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="9df02-122">删除</span><span class="sxs-lookup"><span data-stu-id="9df02-122">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="9df02-123">无</span><span class="sxs-lookup"><span data-stu-id="9df02-123">None</span></span> | <span data-ttu-id="9df02-124">删除 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="9df02-124">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9df02-125">属性</span><span class="sxs-lookup"><span data-stu-id="9df02-125">Properties</span></span>

| <span data-ttu-id="9df02-126">属性</span><span class="sxs-lookup"><span data-stu-id="9df02-126">Property</span></span>     | <span data-ttu-id="9df02-127">类型</span><span class="sxs-lookup"><span data-stu-id="9df02-127">Type</span></span>        | <span data-ttu-id="9df02-128">说明</span><span class="sxs-lookup"><span data-stu-id="9df02-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9df02-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="9df02-129">apiVersion</span></span>|<span data-ttu-id="9df02-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9df02-130">Int32</span></span>|<span data-ttu-id="9df02-131">回调 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="9df02-131">API version for the call back URL.</span></span> <span data-ttu-id="9df02-132">从1开始。</span><span class="sxs-lookup"><span data-stu-id="9df02-132">Start with 1.</span></span>|
|<span data-ttu-id="9df02-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9df02-133">displayName</span></span>|<span data-ttu-id="9df02-134">String</span><span class="sxs-lookup"><span data-stu-id="9df02-134">String</span></span>|<span data-ttu-id="9df02-135">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="9df02-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="9df02-136">技术</span><span class="sxs-lookup"><span data-stu-id="9df02-136">encryption</span></span>|[<span data-ttu-id="9df02-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="9df02-137">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="9df02-138">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="9df02-138">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="9df02-139">isActive</span><span class="sxs-lookup"><span data-stu-id="9df02-139">isActive</span></span>|<span data-ttu-id="9df02-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="9df02-140">Boolean</span></span>|<span data-ttu-id="9df02-141">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="9df02-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="9df02-142">支持</span><span class="sxs-lookup"><span data-stu-id="9df02-142">supports</span></span>|<span data-ttu-id="9df02-143">string</span><span class="sxs-lookup"><span data-stu-id="9df02-143">string</span></span>| <span data-ttu-id="9df02-144">移位支持同步更改通知的实体。</span><span class="sxs-lookup"><span data-stu-id="9df02-144">The Shifts entities supported for synchronous change notifications.</span></span> <span data-ttu-id="9df02-145">班次将回拨到在此处添加的这些实体上的客户端更改上提供的 url。</span><span class="sxs-lookup"><span data-stu-id="9df02-145">Shifts will make a call back to the url provided on client changes on those entities added here.</span></span> <span data-ttu-id="9df02-146">默认情况下，不支持更改通知的任何实体。</span><span class="sxs-lookup"><span data-stu-id="9df02-146">By default, no entities are supported for change notifications.</span></span> <span data-ttu-id="9df02-147">可能的值为 `none` ： `shift` 、 `swapRequest` 、 `openshift` `openShiftRequest` 、、 `userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="9df02-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="9df02-148">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="9df02-148">supportedEntities</span></span>|<span data-ttu-id="9df02-149">string</span><span class="sxs-lookup"><span data-stu-id="9df02-149">string</span></span>| <span data-ttu-id="9df02-150">此属性将替换1.0 版中的 **支持** 。</span><span class="sxs-lookup"><span data-stu-id="9df02-150">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="9df02-151">建议使用此属性，而不 **支持**。</span><span class="sxs-lookup"><span data-stu-id="9df02-151">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="9df02-152">**支持**属性将在 beta 中仍受支持。</span><span class="sxs-lookup"><span data-stu-id="9df02-152">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="9df02-153">可能的值为、、、、 `none` `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` 。</span><span class="sxs-lookup"><span data-stu-id="9df02-153">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="9df02-154">如果选择多个值，则所有值必须以大写形式的第一个字母开头。</span><span class="sxs-lookup"><span data-stu-id="9df02-154">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="9df02-155">url</span><span class="sxs-lookup"><span data-stu-id="9df02-155">url</span></span>|<span data-ttu-id="9df02-156">String</span><span class="sxs-lookup"><span data-stu-id="9df02-156">String</span></span>| <span data-ttu-id="9df02-157">来自倒班服务的回调的劳动力集成 URL。</span><span class="sxs-lookup"><span data-stu-id="9df02-157">Workforce Integration URL for callbacks from the Shifts service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9df02-158">关系</span><span class="sxs-lookup"><span data-stu-id="9df02-158">Relationships</span></span>

<span data-ttu-id="9df02-159">无。</span><span class="sxs-lookup"><span data-stu-id="9df02-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9df02-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9df02-160">JSON representation</span></span>

<span data-ttu-id="9df02-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9df02-161">The following is a JSON representation of the resource.</span></span>

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
  "supports": "string",
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


