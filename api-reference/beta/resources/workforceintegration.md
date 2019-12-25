---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 631f2cc52b9327d77edd6fc5ad48292cf044570f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866488"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="784c4-103">workforceIntegration 资源类型</span><span class="sxs-lookup"><span data-stu-id="784c4-103">workforceIntegration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="784c4-104">员工的一个实例与倒班的集成。</span><span class="sxs-lookup"><span data-stu-id="784c4-104">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="784c4-105">方法</span><span class="sxs-lookup"><span data-stu-id="784c4-105">Methods</span></span>

| <span data-ttu-id="784c4-106">方法</span><span class="sxs-lookup"><span data-stu-id="784c4-106">Method</span></span>       | <span data-ttu-id="784c4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="784c4-107">Return Type</span></span> | <span data-ttu-id="784c4-108">说明</span><span class="sxs-lookup"><span data-stu-id="784c4-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="784c4-109">获取</span><span class="sxs-lookup"><span data-stu-id="784c4-109">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="784c4-110">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="784c4-110">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="784c4-111">读取**workforceIntegration**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="784c4-111">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="784c4-112">更新</span><span class="sxs-lookup"><span data-stu-id="784c4-112">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="784c4-113">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="784c4-113">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="784c4-114">更新**workforceIntegration**对象。</span><span class="sxs-lookup"><span data-stu-id="784c4-114">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="784c4-115">删除</span><span class="sxs-lookup"><span data-stu-id="784c4-115">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="784c4-116">无</span><span class="sxs-lookup"><span data-stu-id="784c4-116">None</span></span> | <span data-ttu-id="784c4-117">删除**workforceIntegration**对象。</span><span class="sxs-lookup"><span data-stu-id="784c4-117">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="784c4-118">属性</span><span class="sxs-lookup"><span data-stu-id="784c4-118">Properties</span></span>

| <span data-ttu-id="784c4-119">属性</span><span class="sxs-lookup"><span data-stu-id="784c4-119">Property</span></span>     | <span data-ttu-id="784c4-120">类型</span><span class="sxs-lookup"><span data-stu-id="784c4-120">Type</span></span>        | <span data-ttu-id="784c4-121">说明</span><span class="sxs-lookup"><span data-stu-id="784c4-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="784c4-122">apiVersion</span><span class="sxs-lookup"><span data-stu-id="784c4-122">apiVersion</span></span>|<span data-ttu-id="784c4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="784c4-123">Int32</span></span>|<span data-ttu-id="784c4-124">回调 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="784c4-124">API version for the call back URL.</span></span> <span data-ttu-id="784c4-125">从1开始。</span><span class="sxs-lookup"><span data-stu-id="784c4-125">Start with 1.</span></span>|
|<span data-ttu-id="784c4-126">displayName</span><span class="sxs-lookup"><span data-stu-id="784c4-126">displayName</span></span>|<span data-ttu-id="784c4-127">String</span><span class="sxs-lookup"><span data-stu-id="784c4-127">String</span></span>|<span data-ttu-id="784c4-128">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="784c4-128">Name of the workforce integration.</span></span>|
|<span data-ttu-id="784c4-129">技术</span><span class="sxs-lookup"><span data-stu-id="784c4-129">encryption</span></span>|[<span data-ttu-id="784c4-130">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="784c4-130">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="784c4-131">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="784c4-131">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="784c4-132">isActive</span><span class="sxs-lookup"><span data-stu-id="784c4-132">isActive</span></span>|<span data-ttu-id="784c4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="784c4-133">Boolean</span></span>|<span data-ttu-id="784c4-134">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="784c4-134">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="784c4-135">支持</span><span class="sxs-lookup"><span data-stu-id="784c4-135">supports</span></span>|<span data-ttu-id="784c4-136">string</span><span class="sxs-lookup"><span data-stu-id="784c4-136">string</span></span>| <span data-ttu-id="784c4-137">可能的值为`none`： `shift`、 `swapRequest`、 `openshift` `openShiftRequest`、、`userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="784c4-137">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="784c4-138">url</span><span class="sxs-lookup"><span data-stu-id="784c4-138">url</span></span>|<span data-ttu-id="784c4-139">String</span><span class="sxs-lookup"><span data-stu-id="784c4-139">String</span></span>| <span data-ttu-id="784c4-140">劳动力集成 URL，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="784c4-140">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="784c4-141">关系</span><span class="sxs-lookup"><span data-stu-id="784c4-141">Relationships</span></span>

<span data-ttu-id="784c4-142">无。</span><span class="sxs-lookup"><span data-stu-id="784c4-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="784c4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="784c4-143">JSON representation</span></span>

<span data-ttu-id="784c4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="784c4-144">The following is a JSON representation of the resource.</span></span>

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
