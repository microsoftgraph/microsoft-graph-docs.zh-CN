---
title: connectorGroup 资源类型
description: 表示应用程序代理连接器组。
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: df3a80c6dfd4004daccfe33045c8775c2e2e6e48
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958806"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="8e408-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e408-103">connectorGroup resource type</span></span>

<span data-ttu-id="8e408-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e408-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e408-105">每个 [Azure AD 应用程序代理](https://aka.ms/whyappproxy) 连接器始终是连接器组的一部分。</span><span class="sxs-lookup"><span data-stu-id="8e408-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="8e408-106">属于同一连接器组的所有连接器都充当高可用性和负载平衡的单独单元。</span><span class="sxs-lookup"><span data-stu-id="8e408-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="8e408-107">如果未创建连接器组，则所有连接器都将是默认组的一部分。</span><span class="sxs-lookup"><span data-stu-id="8e408-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="8e408-108">使用应用程序代理配置应用程序时，还必须指定要为其分配应用程序的连接器组。</span><span class="sxs-lookup"><span data-stu-id="8e408-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="8e408-109">创建连接器组后，可以使用添加连接器将连接器添加或移动到 [连接器组](../api/connectorgroup-post-members.md)。</span><span class="sxs-lookup"><span data-stu-id="8e408-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="8e408-110">您还可以使用 ["添加应用程序](../api/connectorgroup-post-applications.md) "将应用程序分配给连接器组。</span><span class="sxs-lookup"><span data-stu-id="8e408-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="8e408-111">Methods</span><span class="sxs-lookup"><span data-stu-id="8e408-111">Methods</span></span>

| <span data-ttu-id="8e408-112">方法</span><span class="sxs-lookup"><span data-stu-id="8e408-112">Method</span></span>           | <span data-ttu-id="8e408-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="8e408-113">Return Type</span></span>    |<span data-ttu-id="8e408-114">说明</span><span class="sxs-lookup"><span data-stu-id="8e408-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e408-115">列出 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="8e408-116">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e408-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="8e408-117">检索 connectorGroup 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8e408-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="8e408-118">Create connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="8e408-119">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e408-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="8e408-120">创建 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="8e408-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="8e408-121">Get connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="8e408-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="8e408-123">读取 connectorGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e408-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="8e408-124">Update connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="8e408-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="8e408-126">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="8e408-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="8e408-127">Delete connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8e408-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="8e408-128">无</span><span class="sxs-lookup"><span data-stu-id="8e408-128">None</span></span> | <span data-ttu-id="8e408-129">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="8e408-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="8e408-130">必须先从 connectorGroup 中删除所有连接器，然后才能删除 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="8e408-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="8e408-131">List members</span><span class="sxs-lookup"><span data-stu-id="8e408-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="8e408-132">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e408-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="8e408-133">获取连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="8e408-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="8e408-134">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="8e408-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="8e408-135">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e408-135">[application](application.md) collection</span></span>| <span data-ttu-id="8e408-136">获取与 connectorGroup 关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="8e408-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="8e408-137">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="8e408-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="8e408-138">application</span><span class="sxs-lookup"><span data-stu-id="8e408-138">application</span></span>](application.md)| <span data-ttu-id="8e408-139">通过发布到应用程序集合将应用程序与 connectorGroup 关联。</span><span class="sxs-lookup"><span data-stu-id="8e408-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="8e408-140">Add connector</span><span class="sxs-lookup"><span data-stu-id="8e408-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="8e408-141">connector</span><span class="sxs-lookup"><span data-stu-id="8e408-141">connector</span></span>](connector.md)| <span data-ttu-id="8e408-142">通过发布到 connectorGroup 集合将连接器添加到 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="8e408-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e408-143">属性</span><span class="sxs-lookup"><span data-stu-id="8e408-143">Properties</span></span>
| <span data-ttu-id="8e408-144">属性</span><span class="sxs-lookup"><span data-stu-id="8e408-144">Property</span></span>     | <span data-ttu-id="8e408-145">类型</span><span class="sxs-lookup"><span data-stu-id="8e408-145">Type</span></span>   |<span data-ttu-id="8e408-146">说明</span><span class="sxs-lookup"><span data-stu-id="8e408-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e408-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="8e408-147">connectorGroupType</span></span>|<span data-ttu-id="8e408-148">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="8e408-148">connectorGroupType</span></span>| <span data-ttu-id="8e408-149">指示混合代理的类型。</span><span class="sxs-lookup"><span data-stu-id="8e408-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="8e408-150">此预设置由系统设置。</span><span class="sxs-lookup"><span data-stu-id="8e408-150">This pre-set by the system.</span></span> <span data-ttu-id="8e408-151">可能的值是 `applicationProxy` ：。</span><span class="sxs-lookup"><span data-stu-id="8e408-151">Possible values are: `applicationProxy`.</span></span> <span data-ttu-id="8e408-152">只读。</span><span class="sxs-lookup"><span data-stu-id="8e408-152">Read-only.</span></span> |
|<span data-ttu-id="8e408-153">id</span><span class="sxs-lookup"><span data-stu-id="8e408-153">id</span></span>|<span data-ttu-id="8e408-154">string</span><span class="sxs-lookup"><span data-stu-id="8e408-154">string</span></span>| <span data-ttu-id="8e408-155">此 connectorGroup 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8e408-155">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="8e408-156">只读。</span><span class="sxs-lookup"><span data-stu-id="8e408-156">Read-only.</span></span> |
|<span data-ttu-id="8e408-157">isDefault</span><span class="sxs-lookup"><span data-stu-id="8e408-157">isDefault</span></span>|<span data-ttu-id="8e408-158">boolean</span><span class="sxs-lookup"><span data-stu-id="8e408-158">boolean</span></span>| <span data-ttu-id="8e408-159">指示 connectorGroup 是否默认为 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="8e408-159">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="8e408-160">只有一个连接器组可以是默认的 connectorGroup，这由系统预先设置。</span><span class="sxs-lookup"><span data-stu-id="8e408-160">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="8e408-161">只读。</span><span class="sxs-lookup"><span data-stu-id="8e408-161">Read-only.</span></span> |
|<span data-ttu-id="8e408-162">name</span><span class="sxs-lookup"><span data-stu-id="8e408-162">name</span></span>|<span data-ttu-id="8e408-163">string</span><span class="sxs-lookup"><span data-stu-id="8e408-163">string</span></span>| <span data-ttu-id="8e408-164">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="8e408-164">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="8e408-165">region</span><span class="sxs-lookup"><span data-stu-id="8e408-165">region</span></span>|<span data-ttu-id="8e408-166">connectorGroupRegion</span><span class="sxs-lookup"><span data-stu-id="8e408-166">connectorGroupRegion</span></span>| <span data-ttu-id="8e408-167">connectorGroup 分配到的区域，并将优化其流量。</span><span class="sxs-lookup"><span data-stu-id="8e408-167">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="8e408-168">只有未向 connectorGroup **分配连接器** 或应用程序时，才能设置此区域。</span><span class="sxs-lookup"><span data-stu-id="8e408-168">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="8e408-169">可能的值包括：北美 `nam` () 、 (for Europe  `eur` `aus`) 、 (for Australia `asia`) 、 (for Asia `ind`) 、 (for India) `unknownFutureValue` 和 。</span><span class="sxs-lookup"><span data-stu-id="8e408-169">The possible values are: `nam` (for **North America**), `eur` (for Europe), `aus` (for Australia), `asia` (for Asia), `ind` (for India), and `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e408-170">关系</span><span class="sxs-lookup"><span data-stu-id="8e408-170">Relationships</span></span>
| <span data-ttu-id="8e408-171">关系</span><span class="sxs-lookup"><span data-stu-id="8e408-171">Relationship</span></span> | <span data-ttu-id="8e408-172">类型</span><span class="sxs-lookup"><span data-stu-id="8e408-172">Type</span></span>   |<span data-ttu-id="8e408-173">说明</span><span class="sxs-lookup"><span data-stu-id="8e408-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e408-174">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e408-174">applications</span></span>|<span data-ttu-id="8e408-175">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e408-175">[application](application.md) collection</span></span>| <span data-ttu-id="8e408-176">只读。</span><span class="sxs-lookup"><span data-stu-id="8e408-176">Read-only.</span></span> <span data-ttu-id="8e408-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8e408-177">Nullable.</span></span>|
|<span data-ttu-id="8e408-178">members</span><span class="sxs-lookup"><span data-stu-id="8e408-178">members</span></span>|<span data-ttu-id="8e408-179">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e408-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="8e408-p109">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="8e408-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e408-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e408-182">JSON representation</span></span>

<span data-ttu-id="8e408-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e408-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
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



