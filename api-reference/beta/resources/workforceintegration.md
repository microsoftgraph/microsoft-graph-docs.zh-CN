---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa604c7d087d3231dd6ed1c6903a87f80298904b
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895618"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="b5b3b-103">workforceIntegration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5b3b-103">workforceIntegration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5b3b-104">Workforceforce 与倒班的集成实例。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-104">An instance of a workforceforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="b5b3b-105">方法</span><span class="sxs-lookup"><span data-stu-id="b5b3b-105">Methods</span></span>

| <span data-ttu-id="b5b3b-106">方法</span><span class="sxs-lookup"><span data-stu-id="b5b3b-106">Method</span></span>       | <span data-ttu-id="b5b3b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5b3b-107">Return Type</span></span> | <span data-ttu-id="b5b3b-108">说明</span><span class="sxs-lookup"><span data-stu-id="b5b3b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b5b3b-109">获取</span><span class="sxs-lookup"><span data-stu-id="b5b3b-109">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="b5b3b-110">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b5b3b-110">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="b5b3b-111">读取**workforceIntegration**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-111">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="b5b3b-112">更新</span><span class="sxs-lookup"><span data-stu-id="b5b3b-112">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="b5b3b-113">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b5b3b-113">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="b5b3b-114">更新**workforceIntegration**对象。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-114">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="b5b3b-115">删除</span><span class="sxs-lookup"><span data-stu-id="b5b3b-115">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="b5b3b-116">None</span><span class="sxs-lookup"><span data-stu-id="b5b3b-116">None</span></span> | <span data-ttu-id="b5b3b-117">删除**workforceIntegration**对象。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-117">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b5b3b-118">属性</span><span class="sxs-lookup"><span data-stu-id="b5b3b-118">Properties</span></span>

| <span data-ttu-id="b5b3b-119">属性</span><span class="sxs-lookup"><span data-stu-id="b5b3b-119">Property</span></span>     | <span data-ttu-id="b5b3b-120">类型</span><span class="sxs-lookup"><span data-stu-id="b5b3b-120">Type</span></span>        | <span data-ttu-id="b5b3b-121">说明</span><span class="sxs-lookup"><span data-stu-id="b5b3b-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5b3b-122">apiVersion</span><span class="sxs-lookup"><span data-stu-id="b5b3b-122">apiVersion</span></span>|<span data-ttu-id="b5b3b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b5b3b-123">Int32</span></span>|<span data-ttu-id="b5b3b-124">回调 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-124">API version for the call back URL.</span></span> <span data-ttu-id="b5b3b-125">从1开始。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-125">Start with 1.</span></span>|
|<span data-ttu-id="b5b3b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="b5b3b-126">displayName</span></span>|<span data-ttu-id="b5b3b-127">String</span><span class="sxs-lookup"><span data-stu-id="b5b3b-127">String</span></span>|<span data-ttu-id="b5b3b-128">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-128">Name of the workforce integration.</span></span>|
|<span data-ttu-id="b5b3b-129">技术</span><span class="sxs-lookup"><span data-stu-id="b5b3b-129">encryption</span></span>|[<span data-ttu-id="b5b3b-130">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="b5b3b-130">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="b5b3b-131">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-131">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="b5b3b-132">isActive</span><span class="sxs-lookup"><span data-stu-id="b5b3b-132">isActive</span></span>|<span data-ttu-id="b5b3b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5b3b-133">Boolean</span></span>|<span data-ttu-id="b5b3b-134">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-134">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="b5b3b-135">支持</span><span class="sxs-lookup"><span data-stu-id="b5b3b-135">supports</span></span>|<span data-ttu-id="b5b3b-136">string</span><span class="sxs-lookup"><span data-stu-id="b5b3b-136">string</span></span>| <span data-ttu-id="b5b3b-137">可能的值为`none`： `shift`、 `swapRequest`、 `openshift` `openShiftRequest`、、`userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="b5b3b-137">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="b5b3b-138">url</span><span class="sxs-lookup"><span data-stu-id="b5b3b-138">url</span></span>|<span data-ttu-id="b5b3b-139">String</span><span class="sxs-lookup"><span data-stu-id="b5b3b-139">String</span></span>| <span data-ttu-id="b5b3b-140">劳动力集成 URL，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-140">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5b3b-141">关系</span><span class="sxs-lookup"><span data-stu-id="b5b3b-141">Relationships</span></span>

<span data-ttu-id="b5b3b-142">无。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5b3b-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5b3b-143">JSON representation</span></span>

<span data-ttu-id="b5b3b-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5b3b-144">The following is a JSON representation of the resource.</span></span>

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
