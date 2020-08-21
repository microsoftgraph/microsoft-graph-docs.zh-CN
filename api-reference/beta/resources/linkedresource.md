---
title: linkedResource 资源类型
description: 表示 todoTask 的源
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a386cd8ed714a6f7127ea0a872a4170997bb8b9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849905"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="321ab-103">linkedResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="321ab-103">linkedResource resource type</span></span>

<span data-ttu-id="321ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="321ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321ab-105">表示合作伙伴应用程序中与 [todoTask 相关的项目](./todotask.md)。</span><span class="sxs-lookup"><span data-stu-id="321ab-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="321ab-106">例如，创建了任务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="321ab-106">An example is an email that created the task.</span></span> <span data-ttu-id="321ab-107">**linkedResource**对象存储有关该源应用程序的信息，并允许您链接回相关项。</span><span class="sxs-lookup"><span data-stu-id="321ab-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span>

## <a name="methods"></a><span data-ttu-id="321ab-108">方法</span><span class="sxs-lookup"><span data-stu-id="321ab-108">Methods</span></span>
|<span data-ttu-id="321ab-109">方法</span><span class="sxs-lookup"><span data-stu-id="321ab-109">Method</span></span>|<span data-ttu-id="321ab-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="321ab-110">Return type</span></span>|<span data-ttu-id="321ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="321ab-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="321ab-112">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="321ab-112">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="321ab-113">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="321ab-113">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="321ab-114">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="321ab-114">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="321ab-115">创建 linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-115">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="321ab-116">linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-116">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="321ab-117">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="321ab-117">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="321ab-118">获取 linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-118">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="321ab-119">linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-119">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="321ab-120">读取 [linkedResource 对象的属性和](../resources/linkedresource.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="321ab-120">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="321ab-121">更新 linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-121">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="321ab-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="321ab-123">更新 [linkedResource 对象的](../resources/linkedresource.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="321ab-123">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="321ab-124">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="321ab-124">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="321ab-125">无</span><span class="sxs-lookup"><span data-stu-id="321ab-125">None</span></span>|<span data-ttu-id="321ab-126">删除 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="321ab-126">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="321ab-127">属性</span><span class="sxs-lookup"><span data-stu-id="321ab-127">Properties</span></span>
|<span data-ttu-id="321ab-128">属性</span><span class="sxs-lookup"><span data-stu-id="321ab-128">Property</span></span>|<span data-ttu-id="321ab-129">类型</span><span class="sxs-lookup"><span data-stu-id="321ab-129">Type</span></span>|<span data-ttu-id="321ab-130">说明</span><span class="sxs-lookup"><span data-stu-id="321ab-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="321ab-131">applicationName</span><span class="sxs-lookup"><span data-stu-id="321ab-131">applicationName</span></span>|<span data-ttu-id="321ab-132">String</span><span class="sxs-lookup"><span data-stu-id="321ab-132">String</span></span>|<span data-ttu-id="321ab-133">指示发送 linkedResource 的源的应用 **名称的字段**。</span><span class="sxs-lookup"><span data-stu-id="321ab-133">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="321ab-134">displayName</span><span class="sxs-lookup"><span data-stu-id="321ab-134">displayName</span></span>|<span data-ttu-id="321ab-135">String</span><span class="sxs-lookup"><span data-stu-id="321ab-135">String</span></span>|<span data-ttu-id="321ab-136">指示 **linkedResource 标题的域**。</span><span class="sxs-lookup"><span data-stu-id="321ab-136">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="321ab-137">externalId</span><span class="sxs-lookup"><span data-stu-id="321ab-137">externalId</span></span>|<span data-ttu-id="321ab-138">String</span><span class="sxs-lookup"><span data-stu-id="321ab-138">String</span></span>|<span data-ttu-id="321ab-139">与第三方/合作伙伴系统上的此任务相关联的对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="321ab-139">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="321ab-140">id</span><span class="sxs-lookup"><span data-stu-id="321ab-140">id</span></span>|<span data-ttu-id="321ab-141">String</span><span class="sxs-lookup"><span data-stu-id="321ab-141">String</span></span>|<span data-ttu-id="321ab-142">**linkedResource 的服务器生成的**ID。</span><span class="sxs-lookup"><span data-stu-id="321ab-142">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="321ab-143">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="321ab-143">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="321ab-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="321ab-144">webUrl</span></span>|<span data-ttu-id="321ab-145">String</span><span class="sxs-lookup"><span data-stu-id="321ab-145">String</span></span>|<span data-ttu-id="321ab-146">到 **linkedResource 的深度链接**。</span><span class="sxs-lookup"><span data-stu-id="321ab-146">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="321ab-147">关系</span><span class="sxs-lookup"><span data-stu-id="321ab-147">Relationships</span></span>
<span data-ttu-id="321ab-148">无。</span><span class="sxs-lookup"><span data-stu-id="321ab-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="321ab-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="321ab-149">JSON representation</span></span>
<span data-ttu-id="321ab-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="321ab-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```

