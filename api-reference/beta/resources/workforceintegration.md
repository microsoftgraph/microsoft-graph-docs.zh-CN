---
title: workforceIntegration 资源类型
description: 员工与班次集成的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b9e8678a009dab1f6e6cceae8b9ce98d1849cbd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158308"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="84e16-103">workforceIntegration 资源类型</span><span class="sxs-lookup"><span data-stu-id="84e16-103">workforceIntegration resource type</span></span>

<span data-ttu-id="84e16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84e16-105">员工与班次集成的实例。</span><span class="sxs-lookup"><span data-stu-id="84e16-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="84e16-106">方法</span><span class="sxs-lookup"><span data-stu-id="84e16-106">Methods</span></span>

| <span data-ttu-id="84e16-107">方法</span><span class="sxs-lookup"><span data-stu-id="84e16-107">Method</span></span>       | <span data-ttu-id="84e16-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="84e16-108">Return Type</span></span> | <span data-ttu-id="84e16-109">Description</span><span class="sxs-lookup"><span data-stu-id="84e16-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="84e16-110">List</span><span class="sxs-lookup"><span data-stu-id="84e16-110">List</span></span>](../api/workforceintegration-list.md) | <span data-ttu-id="84e16-111">[workforceIntegration](workforceintegration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84e16-111">[workforceIntegration](workforceintegration.md) collection</span></span> | <span data-ttu-id="84e16-112">获取与此 **计划关联的 workforceIntegration** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="84e16-112">Get the list of **workforceIntegration** objects associated with this schedule.</span></span>|
| [<span data-ttu-id="84e16-113">创建</span><span class="sxs-lookup"><span data-stu-id="84e16-113">Create</span></span>](../api/workforceintegration-post.md) | [<span data-ttu-id="84e16-114">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="84e16-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="84e16-115">创建新的 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="84e16-115">Create a new **workforceIntegration** object.</span></span>|
| [<span data-ttu-id="84e16-116">Get</span><span class="sxs-lookup"><span data-stu-id="84e16-116">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="84e16-117">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="84e16-117">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="84e16-118">读取 **workforceIntegration** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84e16-118">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="84e16-119">更新</span><span class="sxs-lookup"><span data-stu-id="84e16-119">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="84e16-120">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="84e16-120">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="84e16-121">更新 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="84e16-121">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="84e16-122">删除</span><span class="sxs-lookup"><span data-stu-id="84e16-122">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="84e16-123">无</span><span class="sxs-lookup"><span data-stu-id="84e16-123">None</span></span> | <span data-ttu-id="84e16-124">删除 **一个 workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="84e16-124">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="84e16-125">属性</span><span class="sxs-lookup"><span data-stu-id="84e16-125">Properties</span></span>

| <span data-ttu-id="84e16-126">属性</span><span class="sxs-lookup"><span data-stu-id="84e16-126">Property</span></span>     | <span data-ttu-id="84e16-127">类型</span><span class="sxs-lookup"><span data-stu-id="84e16-127">Type</span></span>        | <span data-ttu-id="84e16-128">说明</span><span class="sxs-lookup"><span data-stu-id="84e16-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84e16-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="84e16-129">apiVersion</span></span>|<span data-ttu-id="84e16-130">Int32</span><span class="sxs-lookup"><span data-stu-id="84e16-130">Int32</span></span>|<span data-ttu-id="84e16-131">用于回叫 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="84e16-131">API version for the call back URL.</span></span> <span data-ttu-id="84e16-132">从 1 开始。</span><span class="sxs-lookup"><span data-stu-id="84e16-132">Start with 1.</span></span>|
|<span data-ttu-id="84e16-133">displayName</span><span class="sxs-lookup"><span data-stu-id="84e16-133">displayName</span></span>|<span data-ttu-id="84e16-134">String</span><span class="sxs-lookup"><span data-stu-id="84e16-134">String</span></span>|<span data-ttu-id="84e16-135">员工集成的名称。</span><span class="sxs-lookup"><span data-stu-id="84e16-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="84e16-136">加密</span><span class="sxs-lookup"><span data-stu-id="84e16-136">encryption</span></span>|[<span data-ttu-id="84e16-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="84e16-137">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="84e16-138">员工集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="84e16-138">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="84e16-139">isActive</span><span class="sxs-lookup"><span data-stu-id="84e16-139">isActive</span></span>|<span data-ttu-id="84e16-140">布尔</span><span class="sxs-lookup"><span data-stu-id="84e16-140">Boolean</span></span>|<span data-ttu-id="84e16-141">指示此员工集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="84e16-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="84e16-142">supports</span><span class="sxs-lookup"><span data-stu-id="84e16-142">supports</span></span>|<span data-ttu-id="84e16-143">string</span><span class="sxs-lookup"><span data-stu-id="84e16-143">string</span></span>| <span data-ttu-id="84e16-144">同步更改通知支持的 Shifts 实体。</span><span class="sxs-lookup"><span data-stu-id="84e16-144">The Shifts entities supported for synchronous change notifications.</span></span> <span data-ttu-id="84e16-145">Shifts 将调用此处添加的实体上的客户端更改时提供的 URL。</span><span class="sxs-lookup"><span data-stu-id="84e16-145">Shifts will make a call back to the url provided on client changes on those entities added here.</span></span> <span data-ttu-id="84e16-146">默认情况下，更改通知不支持任何实体。</span><span class="sxs-lookup"><span data-stu-id="84e16-146">By default, no entities are supported for change notifications.</span></span> <span data-ttu-id="84e16-147">可能的值是： `none` `shift` ， ， ， `swapRequest` `openshift` ， `openShiftRequest``userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="84e16-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="84e16-148">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="84e16-148">supportedEntities</span></span>|<span data-ttu-id="84e16-149">string</span><span class="sxs-lookup"><span data-stu-id="84e16-149">string</span></span>| <span data-ttu-id="84e16-150">此属性 **将替换** v1.0 中的支持。</span><span class="sxs-lookup"><span data-stu-id="84e16-150">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="84e16-151">我们建议你使用此属性，而不是 **支持**。</span><span class="sxs-lookup"><span data-stu-id="84e16-151">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="84e16-152">**目前，** 支持属性在 beta 版中仍受支持。</span><span class="sxs-lookup"><span data-stu-id="84e16-152">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="84e16-153">可能的值是 `none` `shift` ， ， ， `swapRequest` `openshift` `openShiftRequest` 。 `userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="84e16-153">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="84e16-154">如果选择多个值，则所有值必须以大写字母开头。</span><span class="sxs-lookup"><span data-stu-id="84e16-154">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="84e16-155">url</span><span class="sxs-lookup"><span data-stu-id="84e16-155">url</span></span>|<span data-ttu-id="84e16-156">String</span><span class="sxs-lookup"><span data-stu-id="84e16-156">String</span></span>| <span data-ttu-id="84e16-157">来自班次服务的回调的员工集成 URL。</span><span class="sxs-lookup"><span data-stu-id="84e16-157">Workforce Integration URL for callbacks from the Shifts service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e16-158">关系</span><span class="sxs-lookup"><span data-stu-id="84e16-158">Relationships</span></span>

<span data-ttu-id="84e16-159">无。</span><span class="sxs-lookup"><span data-stu-id="84e16-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84e16-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84e16-160">JSON representation</span></span>

<span data-ttu-id="84e16-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84e16-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration"
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


