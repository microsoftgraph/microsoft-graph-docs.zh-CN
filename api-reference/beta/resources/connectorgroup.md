---
title: connectorGroup 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d57f116adac652cb55a3a270383ddb5c65d8e40f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507469"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="bb274-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb274-103">connectorGroup resource type</span></span>

<span data-ttu-id="bb274-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bb274-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="bb274-105">方法</span><span class="sxs-lookup"><span data-stu-id="bb274-105">Methods</span></span>

| <span data-ttu-id="bb274-106">方法</span><span class="sxs-lookup"><span data-stu-id="bb274-106">Method</span></span>           | <span data-ttu-id="bb274-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb274-107">Return Type</span></span>    |<span data-ttu-id="bb274-108">说明</span><span class="sxs-lookup"><span data-stu-id="bb274-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb274-109">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb274-109">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="bb274-110">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb274-110">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="bb274-111">读取 connectorGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb274-111">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="bb274-112">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="bb274-112">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="bb274-113">application</span><span class="sxs-lookup"><span data-stu-id="bb274-113">application</span></span>](application.md)| <span data-ttu-id="bb274-114">将应用程序与连接器组关联，方法是发布到应用程序集合。</span><span class="sxs-lookup"><span data-stu-id="bb274-114">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="bb274-115">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="bb274-115">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="bb274-116">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb274-116">[application](application.md) collection</span></span>| <span data-ttu-id="bb274-117">获取关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb274-117">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="bb274-118">创建连接器</span><span class="sxs-lookup"><span data-stu-id="bb274-118">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="bb274-119">连接器</span><span class="sxs-lookup"><span data-stu-id="bb274-119">connector</span></span>](connector.md)| <span data-ttu-id="bb274-120">通过发布到 members 集合，将连接器添加到连接器组。</span><span class="sxs-lookup"><span data-stu-id="bb274-120">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="bb274-121">列出成员</span><span class="sxs-lookup"><span data-stu-id="bb274-121">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="bb274-122">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb274-122">[connector](connector.md) collection</span></span>| <span data-ttu-id="bb274-123">获取连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb274-123">Get a connector object collection.</span></span>|
|[<span data-ttu-id="bb274-124">更新</span><span class="sxs-lookup"><span data-stu-id="bb274-124">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="bb274-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="bb274-125">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="bb274-126">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="bb274-126">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="bb274-127">删除</span><span class="sxs-lookup"><span data-stu-id="bb274-127">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="bb274-128">无</span><span class="sxs-lookup"><span data-stu-id="bb274-128">None</span></span> |<span data-ttu-id="bb274-129">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="bb274-129">Delete connectorGroup object.</span></span> <span data-ttu-id="bb274-130">必须删除所有连接器，然后才能删除连接器组。</span><span class="sxs-lookup"><span data-stu-id="bb274-130">All connectors must be remove before a connector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb274-131">属性</span><span class="sxs-lookup"><span data-stu-id="bb274-131">Properties</span></span>
| <span data-ttu-id="bb274-132">属性</span><span class="sxs-lookup"><span data-stu-id="bb274-132">Property</span></span>     | <span data-ttu-id="bb274-133">类型</span><span class="sxs-lookup"><span data-stu-id="bb274-133">Type</span></span>   |<span data-ttu-id="bb274-134">说明</span><span class="sxs-lookup"><span data-stu-id="bb274-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb274-135">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="bb274-135">connectorGroupType</span></span>|<span data-ttu-id="bb274-136">string</span><span class="sxs-lookup"><span data-stu-id="bb274-136">string</span></span>| <span data-ttu-id="bb274-137">将与组一起使用的连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="bb274-137">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="bb274-138">可能的值是`applicationProxy`：。</span><span class="sxs-lookup"><span data-stu-id="bb274-138">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="bb274-139">id</span><span class="sxs-lookup"><span data-stu-id="bb274-139">id</span></span>|<span data-ttu-id="bb274-140">String</span><span class="sxs-lookup"><span data-stu-id="bb274-140">String</span></span>| <span data-ttu-id="bb274-141">ConnectorGroup 的对象 id</span><span class="sxs-lookup"><span data-stu-id="bb274-141">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="bb274-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="bb274-142">isDefault</span></span>|<span data-ttu-id="bb274-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb274-143">Boolean</span></span>| <span data-ttu-id="bb274-144">指示 connectorGroup 是否为默认的连接器组。</span><span class="sxs-lookup"><span data-stu-id="bb274-144">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="bb274-145">只有一个连接器组可以是默认的 connectorGroup，并由系统进行设置。</span><span class="sxs-lookup"><span data-stu-id="bb274-145">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="bb274-146">name</span><span class="sxs-lookup"><span data-stu-id="bb274-146">name</span></span>|<span data-ttu-id="bb274-147">String</span><span class="sxs-lookup"><span data-stu-id="bb274-147">String</span></span>| <span data-ttu-id="bb274-148">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="bb274-148">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb274-149">关系</span><span class="sxs-lookup"><span data-stu-id="bb274-149">Relationships</span></span>
| <span data-ttu-id="bb274-150">关系</span><span class="sxs-lookup"><span data-stu-id="bb274-150">Relationship</span></span> | <span data-ttu-id="bb274-151">类型</span><span class="sxs-lookup"><span data-stu-id="bb274-151">Type</span></span>   |<span data-ttu-id="bb274-152">说明</span><span class="sxs-lookup"><span data-stu-id="bb274-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb274-153">来说</span><span class="sxs-lookup"><span data-stu-id="bb274-153">applications</span></span>|<span data-ttu-id="bb274-154">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb274-154">[application](application.md) collection</span></span>| <span data-ttu-id="bb274-155">只读。</span><span class="sxs-lookup"><span data-stu-id="bb274-155">Read-only.</span></span> <span data-ttu-id="bb274-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="bb274-156">Nullable.</span></span>|
|<span data-ttu-id="bb274-157">members</span><span class="sxs-lookup"><span data-stu-id="bb274-157">members</span></span>|<span data-ttu-id="bb274-158">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb274-158">[connector](connector.md) collection</span></span>| <span data-ttu-id="bb274-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="bb274-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb274-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb274-161">JSON representation</span></span>

<span data-ttu-id="bb274-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb274-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
