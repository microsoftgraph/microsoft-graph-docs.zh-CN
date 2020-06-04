---
title: connectorGroup 资源类型
description: 表示应用程序代理 connectorGroup。
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 446dae5e78878ba9648d532d2696b0bfde496601
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556168"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="ffc7a-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffc7a-103">connectorGroup resource type</span></span>

<span data-ttu-id="ffc7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffc7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffc7a-105">每个[AZURE AD 应用程序代理](https://aka.ms/whyappproxy)连接器始终是连接器组的一部分。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="ffc7a-106">属于同一连接器组的所有连接器充当高可用性和负载平衡的独立单元。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="ffc7a-107">如果不创建连接器组，则所有连接器都将成为默认组的一部分。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="ffc7a-108">在使用应用程序代理配置应用程序时，还必须指定要向其分配应用程序的连接器组。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="ffc7a-109">创建连接器组之后，可以使用 "[添加连接器](../api/connectorgroup-post-members.md)" 将连接器添加或移动到连接器组。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="ffc7a-110">您还可以使用 "[添加应用程序](../api/connectorgroup-post-applications.md)" 将应用程序分配给连接器组。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="ffc7a-111">Methods</span><span class="sxs-lookup"><span data-stu-id="ffc7a-111">Methods</span></span>

| <span data-ttu-id="ffc7a-112">方法</span><span class="sxs-lookup"><span data-stu-id="ffc7a-112">Method</span></span>           | <span data-ttu-id="ffc7a-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffc7a-113">Return Type</span></span>    |<span data-ttu-id="ffc7a-114">说明</span><span class="sxs-lookup"><span data-stu-id="ffc7a-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ffc7a-115">列出 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ffc7a-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="ffc7a-116">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffc7a-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="ffc7a-117">检索 connectorGroup 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="ffc7a-118">获取 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ffc7a-118">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="ffc7a-119">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ffc7a-119">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="ffc7a-120">读取 connectorGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-120">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="ffc7a-121">更新 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ffc7a-121">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="ffc7a-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ffc7a-122">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="ffc7a-123">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-123">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="ffc7a-124">删除 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ffc7a-124">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="ffc7a-125">无</span><span class="sxs-lookup"><span data-stu-id="ffc7a-125">None</span></span> | <span data-ttu-id="ffc7a-126">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-126">Delete a connectorGroup object.</span></span> <span data-ttu-id="ffc7a-127">必须从 connectorGroup 中删除所有连接器，然后才能删除 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-127">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="ffc7a-128">List members</span><span class="sxs-lookup"><span data-stu-id="ffc7a-128">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="ffc7a-129">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffc7a-129">[connector](connector.md) collection</span></span>| <span data-ttu-id="ffc7a-130">获取连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-130">Get a connector object collection.</span></span> |
|[<span data-ttu-id="ffc7a-131">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="ffc7a-131">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="ffc7a-132">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ffc7a-132">[application](application.md) collection</span></span>| <span data-ttu-id="ffc7a-133">获取与 connectorGroup 相关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-133">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="ffc7a-134">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="ffc7a-134">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="ffc7a-135">application</span><span class="sxs-lookup"><span data-stu-id="ffc7a-135">application</span></span>](application.md)| <span data-ttu-id="ffc7a-136">通过发布到应用程序集合，将应用程序与 connectorGroup 相关联。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-136">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="ffc7a-137">添加连接器</span><span class="sxs-lookup"><span data-stu-id="ffc7a-137">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="ffc7a-138">连接器</span><span class="sxs-lookup"><span data-stu-id="ffc7a-138">connector</span></span>](connector.md)| <span data-ttu-id="ffc7a-139">通过发布到 connectorGroup 集合，将连接器添加到 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-139">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="ffc7a-140">属性</span><span class="sxs-lookup"><span data-stu-id="ffc7a-140">Properties</span></span>
| <span data-ttu-id="ffc7a-141">属性</span><span class="sxs-lookup"><span data-stu-id="ffc7a-141">Property</span></span>     | <span data-ttu-id="ffc7a-142">类型</span><span class="sxs-lookup"><span data-stu-id="ffc7a-142">Type</span></span>   |<span data-ttu-id="ffc7a-143">说明</span><span class="sxs-lookup"><span data-stu-id="ffc7a-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffc7a-144">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="ffc7a-144">connectorGroupType</span></span>|<span data-ttu-id="ffc7a-145">string</span><span class="sxs-lookup"><span data-stu-id="ffc7a-145">string</span></span>| <span data-ttu-id="ffc7a-146">指示混合代理的类型。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-146">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="ffc7a-147">此项预设置的系统。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-147">This pre-set by the system.</span></span> <span data-ttu-id="ffc7a-148">只读。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-148">Read-only.</span></span> |
|<span data-ttu-id="ffc7a-149">id</span><span class="sxs-lookup"><span data-stu-id="ffc7a-149">id</span></span>|<span data-ttu-id="ffc7a-150">string</span><span class="sxs-lookup"><span data-stu-id="ffc7a-150">string</span></span>| <span data-ttu-id="ffc7a-151">此 connectorGroup 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-151">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="ffc7a-152">只读。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-152">Read-only.</span></span> |
|<span data-ttu-id="ffc7a-153">isDefault</span><span class="sxs-lookup"><span data-stu-id="ffc7a-153">isDefault</span></span>|<span data-ttu-id="ffc7a-154">boolean</span><span class="sxs-lookup"><span data-stu-id="ffc7a-154">boolean</span></span>| <span data-ttu-id="ffc7a-155">指示 connectorGroup 是否为默认的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-155">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="ffc7a-156">只有一个连接器组可以是默认的 connectorGroup，这是由系统预设置的。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-156">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="ffc7a-157">只读。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-157">Read-only.</span></span> |
|<span data-ttu-id="ffc7a-158">name</span><span class="sxs-lookup"><span data-stu-id="ffc7a-158">name</span></span>|<span data-ttu-id="ffc7a-159">string</span><span class="sxs-lookup"><span data-stu-id="ffc7a-159">string</span></span>| <span data-ttu-id="ffc7a-160">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-160">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="ffc7a-161">范围</span><span class="sxs-lookup"><span data-stu-id="ffc7a-161">region</span></span>|<span data-ttu-id="ffc7a-162">string</span><span class="sxs-lookup"><span data-stu-id="ffc7a-162">string</span></span>| <span data-ttu-id="ffc7a-163">向其分配 connectorGroup 的区域并将为其优化流量。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-163">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="ffc7a-164">仅当未向 connectorGroup 分配**连接器或应用程序**时，才能设置此区域。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-164">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="ffc7a-165">可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-165">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="ffc7a-166">可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-166">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffc7a-167">关系</span><span class="sxs-lookup"><span data-stu-id="ffc7a-167">Relationships</span></span>
| <span data-ttu-id="ffc7a-168">关系</span><span class="sxs-lookup"><span data-stu-id="ffc7a-168">Relationship</span></span> | <span data-ttu-id="ffc7a-169">类型</span><span class="sxs-lookup"><span data-stu-id="ffc7a-169">Type</span></span>   |<span data-ttu-id="ffc7a-170">说明</span><span class="sxs-lookup"><span data-stu-id="ffc7a-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffc7a-171">来说</span><span class="sxs-lookup"><span data-stu-id="ffc7a-171">applications</span></span>|<span data-ttu-id="ffc7a-172">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ffc7a-172">[application](application.md) collection</span></span>| <span data-ttu-id="ffc7a-173">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-173">Read-only.</span></span> <span data-ttu-id="ffc7a-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-174">Nullable.</span></span>|
|<span data-ttu-id="ffc7a-175">members</span><span class="sxs-lookup"><span data-stu-id="ffc7a-175">members</span></span>|<span data-ttu-id="ffc7a-176">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffc7a-176">[connector](connector.md) collection</span></span>| <span data-ttu-id="ffc7a-p109">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffc7a-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffc7a-179">JSON representation</span></span>

<span data-ttu-id="ffc7a-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffc7a-180">The following is a JSON representation of the resource.</span></span>

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
