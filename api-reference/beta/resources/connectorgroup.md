---
title: connectorGroup 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 211efe5d8caae57457a6a5cc4fa95d145cd176f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823189"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="c054b-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="c054b-103">connectorGroup resource type</span></span>

> <span data-ttu-id="c054b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c054b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c054b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c054b-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="c054b-106">方法</span><span class="sxs-lookup"><span data-stu-id="c054b-106">Methods</span></span>

| <span data-ttu-id="c054b-107">方法</span><span class="sxs-lookup"><span data-stu-id="c054b-107">Method</span></span>           | <span data-ttu-id="c054b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c054b-108">Return Type</span></span>    |<span data-ttu-id="c054b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c054b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c054b-110">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c054b-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="c054b-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c054b-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="c054b-112">读取属性和 connectorGroup 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c054b-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="c054b-113">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="c054b-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="c054b-114">application</span><span class="sxs-lookup"><span data-stu-id="c054b-114">application</span></span>](application.md)| <span data-ttu-id="c054b-115">将应用程序关联连接器组与发布到应用程序集合。</span><span class="sxs-lookup"><span data-stu-id="c054b-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="c054b-116">应用程序列表</span><span class="sxs-lookup"><span data-stu-id="c054b-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="c054b-117">[应用程序](application.md)集合</span><span class="sxs-lookup"><span data-stu-id="c054b-117">[application](application.md) collection</span></span>| <span data-ttu-id="c054b-118">获取关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="c054b-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="c054b-119">创建连接器</span><span class="sxs-lookup"><span data-stu-id="c054b-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="c054b-120">连接器</span><span class="sxs-lookup"><span data-stu-id="c054b-120">connector</span></span>](connector.md)| <span data-ttu-id="c054b-121">通过投递到 members 集合添加到组连接器的连接器。</span><span class="sxs-lookup"><span data-stu-id="c054b-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="c054b-122">列出成员</span><span class="sxs-lookup"><span data-stu-id="c054b-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="c054b-123">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="c054b-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="c054b-124">获取一个连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="c054b-124">Get a connector object collection.</span></span>|
|[<span data-ttu-id="c054b-125">Update</span><span class="sxs-lookup"><span data-stu-id="c054b-125">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="c054b-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c054b-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="c054b-127">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="c054b-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="c054b-128">删除</span><span class="sxs-lookup"><span data-stu-id="c054b-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="c054b-129">无</span><span class="sxs-lookup"><span data-stu-id="c054b-129">None</span></span> |<span data-ttu-id="c054b-130">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="c054b-130">Delete connectorGroup object.</span></span> <span data-ttu-id="c054b-131">可以删除连接器组之前必须删除所有连接线。</span><span class="sxs-lookup"><span data-stu-id="c054b-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="c054b-132">属性</span><span class="sxs-lookup"><span data-stu-id="c054b-132">Properties</span></span>
| <span data-ttu-id="c054b-133">属性</span><span class="sxs-lookup"><span data-stu-id="c054b-133">Property</span></span>     | <span data-ttu-id="c054b-134">类型</span><span class="sxs-lookup"><span data-stu-id="c054b-134">Type</span></span>   |<span data-ttu-id="c054b-135">Description</span><span class="sxs-lookup"><span data-stu-id="c054b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c054b-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="c054b-136">connectorGroupType</span></span>|<span data-ttu-id="c054b-137">string</span><span class="sxs-lookup"><span data-stu-id="c054b-137">string</span></span>| <span data-ttu-id="c054b-138">将使用与组的连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="c054b-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="c054b-139">可能的值为： `applicationProxy`。</span><span class="sxs-lookup"><span data-stu-id="c054b-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="c054b-140">id</span><span class="sxs-lookup"><span data-stu-id="c054b-140">id</span></span>|<span data-ttu-id="c054b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c054b-141">String</span></span>| <span data-ttu-id="c054b-142">ConnectorGroup 对象 id</span><span class="sxs-lookup"><span data-stu-id="c054b-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="c054b-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="c054b-143">isDefault</span></span>|<span data-ttu-id="c054b-144">布尔</span><span class="sxs-lookup"><span data-stu-id="c054b-144">Boolean</span></span>| <span data-ttu-id="c054b-145">指示 connectorGroup 是默认连接器组。</span><span class="sxs-lookup"><span data-stu-id="c054b-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="c054b-146">仅限单个连接器组可以是默认 connectorGroup 并且由系统设置。</span><span class="sxs-lookup"><span data-stu-id="c054b-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="c054b-147">name</span><span class="sxs-lookup"><span data-stu-id="c054b-147">name</span></span>|<span data-ttu-id="c054b-148">字符串</span><span class="sxs-lookup"><span data-stu-id="c054b-148">String</span></span>| <span data-ttu-id="c054b-149">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="c054b-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c054b-150">Relationships</span><span class="sxs-lookup"><span data-stu-id="c054b-150">Relationships</span></span>
| <span data-ttu-id="c054b-151">关系</span><span class="sxs-lookup"><span data-stu-id="c054b-151">Relationship</span></span> | <span data-ttu-id="c054b-152">类型</span><span class="sxs-lookup"><span data-stu-id="c054b-152">Type</span></span>   |<span data-ttu-id="c054b-153">Description</span><span class="sxs-lookup"><span data-stu-id="c054b-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c054b-154">应用程序</span><span class="sxs-lookup"><span data-stu-id="c054b-154">applications</span></span>|<span data-ttu-id="c054b-155">[应用程序](application.md)集合</span><span class="sxs-lookup"><span data-stu-id="c054b-155">[application](application.md) collection</span></span>| <span data-ttu-id="c054b-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c054b-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c054b-158">members</span><span class="sxs-lookup"><span data-stu-id="c054b-158">members</span></span>|<span data-ttu-id="c054b-159">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="c054b-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="c054b-p106">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c054b-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c054b-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c054b-162">JSON representation</span></span>

<span data-ttu-id="c054b-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c054b-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
