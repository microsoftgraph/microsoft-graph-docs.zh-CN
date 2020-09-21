---
title: linkedResource 资源类型
description: 表示 todoTask 的源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3cbfaa0bf809a1996fe7a7c7df7014324406bcf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058107"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="897e6-103">linkedResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="897e6-103">linkedResource resource type</span></span>

<span data-ttu-id="897e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="897e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="897e6-105">表示与 [todoTask](./todotask.md)相关的合作伙伴应用程序中的项。</span><span class="sxs-lookup"><span data-stu-id="897e6-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="897e6-106">例如，创建任务的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="897e6-106">An example is an email that created the task.</span></span> <span data-ttu-id="897e6-107">**LinkedResource**对象存储有关该源应用程序的信息，并允许您链接回相关项目。</span><span class="sxs-lookup"><span data-stu-id="897e6-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span>

## <a name="methods"></a><span data-ttu-id="897e6-108">方法</span><span class="sxs-lookup"><span data-stu-id="897e6-108">Methods</span></span>
|<span data-ttu-id="897e6-109">方法</span><span class="sxs-lookup"><span data-stu-id="897e6-109">Method</span></span>|<span data-ttu-id="897e6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="897e6-110">Return type</span></span>|<span data-ttu-id="897e6-111">说明</span><span class="sxs-lookup"><span data-stu-id="897e6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="897e6-112">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="897e6-112">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="897e6-113">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="897e6-113">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="897e6-114">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="897e6-114">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="897e6-115">创建 linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-115">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="897e6-116">linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-116">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="897e6-117">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="897e6-117">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="897e6-118">获取 linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-118">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="897e6-119">linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-119">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="897e6-120">读取 [linkedResource](../resources/linkedresource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="897e6-120">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="897e6-121">更新 linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-121">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="897e6-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="897e6-123">更新 [linkedResource](../resources/linkedresource.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="897e6-123">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="897e6-124">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="897e6-124">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="897e6-125">无</span><span class="sxs-lookup"><span data-stu-id="897e6-125">None</span></span>|<span data-ttu-id="897e6-126">删除一个 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="897e6-126">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="897e6-127">属性</span><span class="sxs-lookup"><span data-stu-id="897e6-127">Properties</span></span>
|<span data-ttu-id="897e6-128">属性</span><span class="sxs-lookup"><span data-stu-id="897e6-128">Property</span></span>|<span data-ttu-id="897e6-129">类型</span><span class="sxs-lookup"><span data-stu-id="897e6-129">Type</span></span>|<span data-ttu-id="897e6-130">说明</span><span class="sxs-lookup"><span data-stu-id="897e6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="897e6-131">applicationName</span><span class="sxs-lookup"><span data-stu-id="897e6-131">applicationName</span></span>|<span data-ttu-id="897e6-132">String</span><span class="sxs-lookup"><span data-stu-id="897e6-132">String</span></span>|<span data-ttu-id="897e6-133">指示发送 **linkedResource**的源的应用程序名称的字段。</span><span class="sxs-lookup"><span data-stu-id="897e6-133">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="897e6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="897e6-134">displayName</span></span>|<span data-ttu-id="897e6-135">字符串</span><span class="sxs-lookup"><span data-stu-id="897e6-135">String</span></span>|<span data-ttu-id="897e6-136">指示 **linkedResource**的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="897e6-136">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="897e6-137">externalId</span><span class="sxs-lookup"><span data-stu-id="897e6-137">externalId</span></span>|<span data-ttu-id="897e6-138">String</span><span class="sxs-lookup"><span data-stu-id="897e6-138">String</span></span>|<span data-ttu-id="897e6-139">与第三方/合作伙伴系统上的此任务相关联的对象的 Id。</span><span class="sxs-lookup"><span data-stu-id="897e6-139">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="897e6-140">id</span><span class="sxs-lookup"><span data-stu-id="897e6-140">id</span></span>|<span data-ttu-id="897e6-141">字符串</span><span class="sxs-lookup"><span data-stu-id="897e6-141">String</span></span>|<span data-ttu-id="897e6-142">服务器为 **linkedResource**生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="897e6-142">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="897e6-143">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="897e6-143">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="897e6-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="897e6-144">webUrl</span></span>|<span data-ttu-id="897e6-145">String</span><span class="sxs-lookup"><span data-stu-id="897e6-145">String</span></span>|<span data-ttu-id="897e6-146">指向 **linkedResource**的深层链接。</span><span class="sxs-lookup"><span data-stu-id="897e6-146">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="897e6-147">关系</span><span class="sxs-lookup"><span data-stu-id="897e6-147">Relationships</span></span>
<span data-ttu-id="897e6-148">无。</span><span class="sxs-lookup"><span data-stu-id="897e6-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="897e6-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="897e6-149">JSON representation</span></span>
<span data-ttu-id="897e6-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="897e6-150">The following is a JSON representation of the resource.</span></span>
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



