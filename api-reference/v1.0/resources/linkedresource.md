---
title: linkedResource 资源类型
description: 表示 todoTask 的源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 70303742db1dabb866585be7099cb222f8a428bd
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797251"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="a81e1-103">linkedResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a81e1-103">linkedResource resource type</span></span>

<span data-ttu-id="a81e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a81e1-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="a81e1-105">表示与 [todoTask](./todotask.md)相关的合作伙伴应用程序中的项。</span><span class="sxs-lookup"><span data-stu-id="a81e1-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="a81e1-106">例如，创建任务的位置的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a81e1-106">An example is an email from where the task was created.</span></span> <span data-ttu-id="a81e1-107">**LinkedResource** 对象存储有关该源应用程序的信息，并允许您链接回相关项目。</span><span class="sxs-lookup"><span data-stu-id="a81e1-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span> <span data-ttu-id="a81e1-108">您可以在任务详细信息视图中查看 **linkedResource** ，如下所示。</span><span class="sxs-lookup"><span data-stu-id="a81e1-108">You can see the **linkedResource** in the task details view, as shown.</span></span>

![任务详细信息窗格中的链接资源](/graph/images/todo-linkedresource-taskdetail.png)

<span data-ttu-id="a81e1-110">有些 **linkedResource** 对象不与任何 web url 相关联，在这种情况下，不需要 **webUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="a81e1-110">Some **linkedResource** objects are not associated with any web URLs, in which case, the **webUrl** property is not required.</span></span> <span data-ttu-id="a81e1-111">例如，链接的项可以来自自定义的业务应用程序或本机平台应用程序，例如移动电话上的 SMS 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a81e1-111">For example, the linked item can be from a custom business app or native platform app, such as an SMS app on a mobile phone.</span></span> <span data-ttu-id="a81e1-112">以下是 **linkedResource** 的显示方式和不带 URL 的显示方式。</span><span class="sxs-lookup"><span data-stu-id="a81e1-112">Here is how a **linkedResource** appears with and without a URL.</span></span>

![具有和不具有 URL 的链接的资源](/graph/images/todo-linkedresource.png)

## <a name="methods"></a><span data-ttu-id="a81e1-114">方法</span><span class="sxs-lookup"><span data-stu-id="a81e1-114">Methods</span></span>
|<span data-ttu-id="a81e1-115">方法</span><span class="sxs-lookup"><span data-stu-id="a81e1-115">Method</span></span>|<span data-ttu-id="a81e1-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="a81e1-116">Return type</span></span>|<span data-ttu-id="a81e1-117">说明</span><span class="sxs-lookup"><span data-stu-id="a81e1-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a81e1-118">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="a81e1-118">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="a81e1-119">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a81e1-119">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="a81e1-120">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="a81e1-120">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="a81e1-121">创建 linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-121">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="a81e1-122">linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="a81e1-123">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="a81e1-123">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="a81e1-124">获取 linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-124">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="a81e1-125">linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-125">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="a81e1-126">读取 [linkedResource](../resources/linkedresource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a81e1-126">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="a81e1-127">更新 linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-127">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="a81e1-128">linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-128">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="a81e1-129">更新 [linkedResource](../resources/linkedresource.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a81e1-129">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="a81e1-130">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="a81e1-130">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="a81e1-131">无</span><span class="sxs-lookup"><span data-stu-id="a81e1-131">None</span></span>|<span data-ttu-id="a81e1-132">删除一个 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a81e1-132">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a81e1-133">属性</span><span class="sxs-lookup"><span data-stu-id="a81e1-133">Properties</span></span>
|<span data-ttu-id="a81e1-134">属性</span><span class="sxs-lookup"><span data-stu-id="a81e1-134">Property</span></span>|<span data-ttu-id="a81e1-135">类型</span><span class="sxs-lookup"><span data-stu-id="a81e1-135">Type</span></span>|<span data-ttu-id="a81e1-136">说明</span><span class="sxs-lookup"><span data-stu-id="a81e1-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a81e1-137">applicationName</span><span class="sxs-lookup"><span data-stu-id="a81e1-137">applicationName</span></span>|<span data-ttu-id="a81e1-138">String</span><span class="sxs-lookup"><span data-stu-id="a81e1-138">String</span></span>|<span data-ttu-id="a81e1-139">指示发送 **linkedResource** 的源的应用程序名称的字段。</span><span class="sxs-lookup"><span data-stu-id="a81e1-139">Field indicating the app name of the source that is sending the **linkedResource** .</span></span>|
|<span data-ttu-id="a81e1-140">displayName</span><span class="sxs-lookup"><span data-stu-id="a81e1-140">displayName</span></span>|<span data-ttu-id="a81e1-141">String</span><span class="sxs-lookup"><span data-stu-id="a81e1-141">String</span></span>|<span data-ttu-id="a81e1-142">指示 **linkedResource** 的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="a81e1-142">Field indicating the title of the **linkedResource** .</span></span>|
|<span data-ttu-id="a81e1-143">externalId</span><span class="sxs-lookup"><span data-stu-id="a81e1-143">externalId</span></span>|<span data-ttu-id="a81e1-144">String</span><span class="sxs-lookup"><span data-stu-id="a81e1-144">String</span></span>|<span data-ttu-id="a81e1-145">与第三方/合作伙伴系统上的此任务相关联的对象的 Id。</span><span class="sxs-lookup"><span data-stu-id="a81e1-145">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="a81e1-146">id</span><span class="sxs-lookup"><span data-stu-id="a81e1-146">id</span></span>|<span data-ttu-id="a81e1-147">String</span><span class="sxs-lookup"><span data-stu-id="a81e1-147">String</span></span>|<span data-ttu-id="a81e1-148">服务器为 **linkedResource** 生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="a81e1-148">Server generated ID for the **linkedResource** .</span></span> <span data-ttu-id="a81e1-149">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="a81e1-149">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="a81e1-150">WebUrl</span><span class="sxs-lookup"><span data-stu-id="a81e1-150">webUrl</span></span>|<span data-ttu-id="a81e1-151">String</span><span class="sxs-lookup"><span data-stu-id="a81e1-151">String</span></span>|<span data-ttu-id="a81e1-152">指向 **linkedResource** 的深层链接。</span><span class="sxs-lookup"><span data-stu-id="a81e1-152">Deep link to the **linkedResource** .</span></span>|

## <a name="relationships"></a><span data-ttu-id="a81e1-153">关系</span><span class="sxs-lookup"><span data-stu-id="a81e1-153">Relationships</span></span>
<span data-ttu-id="a81e1-154">无。</span><span class="sxs-lookup"><span data-stu-id="a81e1-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a81e1-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a81e1-155">JSON representation</span></span>
<span data-ttu-id="a81e1-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a81e1-156">The following is a JSON representation of the resource.</span></span>
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



