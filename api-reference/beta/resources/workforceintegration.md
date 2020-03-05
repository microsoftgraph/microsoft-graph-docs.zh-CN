---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e836a4346fe5e31f39c1f6383acbf78530ae9e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519083"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="972c0-103">workforceIntegration 资源类型</span><span class="sxs-lookup"><span data-stu-id="972c0-103">workforceIntegration resource type</span></span>

<span data-ttu-id="972c0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="972c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="972c0-105">员工的一个实例与倒班的集成。</span><span class="sxs-lookup"><span data-stu-id="972c0-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="972c0-106">方法</span><span class="sxs-lookup"><span data-stu-id="972c0-106">Methods</span></span>

| <span data-ttu-id="972c0-107">方法</span><span class="sxs-lookup"><span data-stu-id="972c0-107">Method</span></span>       | <span data-ttu-id="972c0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="972c0-108">Return Type</span></span> | <span data-ttu-id="972c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="972c0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="972c0-110">获取</span><span class="sxs-lookup"><span data-stu-id="972c0-110">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="972c0-111">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="972c0-111">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="972c0-112">读取**workforceIntegration**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="972c0-112">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="972c0-113">更新</span><span class="sxs-lookup"><span data-stu-id="972c0-113">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="972c0-114">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="972c0-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="972c0-115">更新**workforceIntegration**对象。</span><span class="sxs-lookup"><span data-stu-id="972c0-115">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="972c0-116">删除</span><span class="sxs-lookup"><span data-stu-id="972c0-116">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="972c0-117">无</span><span class="sxs-lookup"><span data-stu-id="972c0-117">None</span></span> | <span data-ttu-id="972c0-118">删除**workforceIntegration**对象。</span><span class="sxs-lookup"><span data-stu-id="972c0-118">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="972c0-119">属性</span><span class="sxs-lookup"><span data-stu-id="972c0-119">Properties</span></span>

| <span data-ttu-id="972c0-120">属性</span><span class="sxs-lookup"><span data-stu-id="972c0-120">Property</span></span>     | <span data-ttu-id="972c0-121">类型</span><span class="sxs-lookup"><span data-stu-id="972c0-121">Type</span></span>        | <span data-ttu-id="972c0-122">说明</span><span class="sxs-lookup"><span data-stu-id="972c0-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="972c0-123">apiVersion</span><span class="sxs-lookup"><span data-stu-id="972c0-123">apiVersion</span></span>|<span data-ttu-id="972c0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="972c0-124">Int32</span></span>|<span data-ttu-id="972c0-125">回调 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="972c0-125">API version for the call back URL.</span></span> <span data-ttu-id="972c0-126">从1开始。</span><span class="sxs-lookup"><span data-stu-id="972c0-126">Start with 1.</span></span>|
|<span data-ttu-id="972c0-127">displayName</span><span class="sxs-lookup"><span data-stu-id="972c0-127">displayName</span></span>|<span data-ttu-id="972c0-128">String</span><span class="sxs-lookup"><span data-stu-id="972c0-128">String</span></span>|<span data-ttu-id="972c0-129">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="972c0-129">Name of the workforce integration.</span></span>|
|<span data-ttu-id="972c0-130">技术</span><span class="sxs-lookup"><span data-stu-id="972c0-130">encryption</span></span>|[<span data-ttu-id="972c0-131">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="972c0-131">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="972c0-132">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="972c0-132">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="972c0-133">isActive</span><span class="sxs-lookup"><span data-stu-id="972c0-133">isActive</span></span>|<span data-ttu-id="972c0-134">布尔</span><span class="sxs-lookup"><span data-stu-id="972c0-134">Boolean</span></span>|<span data-ttu-id="972c0-135">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="972c0-135">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="972c0-136">支持</span><span class="sxs-lookup"><span data-stu-id="972c0-136">supports</span></span>|<span data-ttu-id="972c0-137">string</span><span class="sxs-lookup"><span data-stu-id="972c0-137">string</span></span>| <span data-ttu-id="972c0-138">可能的值为`none`： `shift`、 `swapRequest`、 `openshift` `openShiftRequest`、、`userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="972c0-138">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="972c0-139">url</span><span class="sxs-lookup"><span data-stu-id="972c0-139">url</span></span>|<span data-ttu-id="972c0-140">String</span><span class="sxs-lookup"><span data-stu-id="972c0-140">String</span></span>| <span data-ttu-id="972c0-141">劳动力集成 URL，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="972c0-141">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="972c0-142">关系</span><span class="sxs-lookup"><span data-stu-id="972c0-142">Relationships</span></span>

<span data-ttu-id="972c0-143">无。</span><span class="sxs-lookup"><span data-stu-id="972c0-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="972c0-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="972c0-144">JSON representation</span></span>

<span data-ttu-id="972c0-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="972c0-145">The following is a JSON representation of the resource.</span></span>

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
