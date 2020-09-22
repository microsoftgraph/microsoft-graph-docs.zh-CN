---
title: connectorGroup 资源类型
description: 表示应用程序代理 connectorGroup。
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: ec56137fab8a929ae3823dcdd339ea6e3b8e174b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027144"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="1a1e1-103">connectorGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a1e1-103">connectorGroup resource type</span></span>

<span data-ttu-id="1a1e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a1e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a1e1-105">每个 [AZURE AD 应用程序代理](https://aka.ms/whyappproxy) 连接器始终是连接器组的一部分。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-105">Each [Azure AD Application Proxy](https://aka.ms/whyappproxy) connector is always part of a connector group.</span></span> <span data-ttu-id="1a1e1-106">属于同一连接器组的所有连接器充当高可用性和负载平衡的独立单元。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-106">All the connectors that belong to the same connector group act as a separate unit for high-availability and load balancing.</span></span> <span data-ttu-id="1a1e1-107">如果不创建连接器组，则所有连接器都将成为默认组的一部分。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-107">If you don't create connector groups, all your connectors will be part of the default group.</span></span> <span data-ttu-id="1a1e1-108">在使用应用程序代理配置应用程序时，还必须指定要向其分配应用程序的连接器组。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-108">When configuring an application with Application Proxy, you must also specify which connector group to assign the application to.</span></span>

<span data-ttu-id="1a1e1-109">创建连接器组之后，可以使用 " [添加连接器](../api/connectorgroup-post-members.md)" 将连接器添加或移动到连接器组。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-109">After a connector group is created, you can add or move connectors to the connector group by using [Add connector](../api/connectorgroup-post-members.md).</span></span> <span data-ttu-id="1a1e1-110">您还可以使用 " [添加应用程序](../api/connectorgroup-post-applications.md) " 将应用程序分配给连接器组。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-110">You can also use [Add application](../api/connectorgroup-post-applications.md) to assign an application to a connector group.</span></span>

## <a name="methods"></a><span data-ttu-id="1a1e1-111">方法</span><span class="sxs-lookup"><span data-stu-id="1a1e1-111">Methods</span></span>

| <span data-ttu-id="1a1e1-112">方法</span><span class="sxs-lookup"><span data-stu-id="1a1e1-112">Method</span></span>           | <span data-ttu-id="1a1e1-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a1e1-113">Return Type</span></span>    |<span data-ttu-id="1a1e1-114">说明</span><span class="sxs-lookup"><span data-stu-id="1a1e1-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a1e1-115">列出 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-115">List connectorGroup</span></span>](../api/connectorgroup-list.md) |<span data-ttu-id="1a1e1-116">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a1e1-116">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="1a1e1-117">检索 connectorGroup 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-117">Retrieve a list of connectorGroup objects.</span></span> |
|[<span data-ttu-id="1a1e1-118">Create connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-118">Create connectorGroup</span></span>](../api/connectorgroup-post.md) |<span data-ttu-id="1a1e1-119">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a1e1-119">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="1a1e1-120">创建 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-120">Create a connectorGroup object.</span></span> |
|[<span data-ttu-id="1a1e1-121">Get connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-121">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="1a1e1-122">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-122">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="1a1e1-123">读取 connectorGroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-123">Read properties and relationships of a connectorGroup object.</span></span> |
|[<span data-ttu-id="1a1e1-124">Update connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-124">Update connectorGroup</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="1a1e1-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-125">connectorGroup</span></span>](connectorgroup.md)| <span data-ttu-id="1a1e1-126">更新 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-126">Update a connectorGroup object.</span></span> |
|[<span data-ttu-id="1a1e1-127">Delete connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a1e1-127">Delete connectorGroup</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="1a1e1-128">无</span><span class="sxs-lookup"><span data-stu-id="1a1e1-128">None</span></span> | <span data-ttu-id="1a1e1-129">删除 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-129">Delete a connectorGroup object.</span></span> <span data-ttu-id="1a1e1-130">必须从 connectorGroup 中删除所有连接器，然后才能删除 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-130">All connectors must be removed from the connectorGroup before a connectorGroup can be deleted.</span></span> |
|[<span data-ttu-id="1a1e1-131">List members</span><span class="sxs-lookup"><span data-stu-id="1a1e1-131">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="1a1e1-132">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a1e1-132">[connector](connector.md) collection</span></span>| <span data-ttu-id="1a1e1-133">获取连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-133">Get a connector object collection.</span></span> |
|[<span data-ttu-id="1a1e1-134">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="1a1e1-134">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="1a1e1-135">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a1e1-135">[application](application.md) collection</span></span>| <span data-ttu-id="1a1e1-136">获取与 connectorGroup 相关联的应用程序对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-136">Get the application object collection associated with the connectorGroup.</span></span> |
|[<span data-ttu-id="1a1e1-137">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="1a1e1-137">Add application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="1a1e1-138">application</span><span class="sxs-lookup"><span data-stu-id="1a1e1-138">application</span></span>](application.md)| <span data-ttu-id="1a1e1-139">通过发布到应用程序集合，将应用程序与 connectorGroup 相关联。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-139">Associate an application with the connectorGroup by posting to the applications collection.</span></span> |
|[<span data-ttu-id="1a1e1-140">Add connector</span><span class="sxs-lookup"><span data-stu-id="1a1e1-140">Add connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="1a1e1-141">连接器</span><span class="sxs-lookup"><span data-stu-id="1a1e1-141">connector</span></span>](connector.md)| <span data-ttu-id="1a1e1-142">通过发布到 connectorGroup 集合，将连接器添加到 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-142">Add a connector to the connectorGroup by posting to the connectorGroup collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a1e1-143">属性</span><span class="sxs-lookup"><span data-stu-id="1a1e1-143">Properties</span></span>
| <span data-ttu-id="1a1e1-144">属性</span><span class="sxs-lookup"><span data-stu-id="1a1e1-144">Property</span></span>     | <span data-ttu-id="1a1e1-145">类型</span><span class="sxs-lookup"><span data-stu-id="1a1e1-145">Type</span></span>   |<span data-ttu-id="1a1e1-146">说明</span><span class="sxs-lookup"><span data-stu-id="1a1e1-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1e1-147">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="1a1e1-147">connectorGroupType</span></span>|<span data-ttu-id="1a1e1-148">string</span><span class="sxs-lookup"><span data-stu-id="1a1e1-148">string</span></span>| <span data-ttu-id="1a1e1-149">指示混合代理的类型。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-149">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="1a1e1-150">此项预设置的系统。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-150">This pre-set by the system.</span></span> <span data-ttu-id="1a1e1-151">只读。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-151">Read-only.</span></span> |
|<span data-ttu-id="1a1e1-152">id</span><span class="sxs-lookup"><span data-stu-id="1a1e1-152">id</span></span>|<span data-ttu-id="1a1e1-153">string</span><span class="sxs-lookup"><span data-stu-id="1a1e1-153">string</span></span>| <span data-ttu-id="1a1e1-154">此 connectorGroup 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-154">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="1a1e1-155">只读。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-155">Read-only.</span></span> |
|<span data-ttu-id="1a1e1-156">isDefault</span><span class="sxs-lookup"><span data-stu-id="1a1e1-156">isDefault</span></span>|<span data-ttu-id="1a1e1-157">boolean</span><span class="sxs-lookup"><span data-stu-id="1a1e1-157">boolean</span></span>| <span data-ttu-id="1a1e1-158">指示 connectorGroup 是否为默认的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-158">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="1a1e1-159">只有一个连接器组可以是默认的 connectorGroup，这是由系统预设置的。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-159">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> <span data-ttu-id="1a1e1-160">只读。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-160">Read-only.</span></span> |
|<span data-ttu-id="1a1e1-161">name</span><span class="sxs-lookup"><span data-stu-id="1a1e1-161">name</span></span>|<span data-ttu-id="1a1e1-162">string</span><span class="sxs-lookup"><span data-stu-id="1a1e1-162">string</span></span>| <span data-ttu-id="1a1e1-163">与 connectorGroup 关联的名称。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-163">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="1a1e1-164">范围</span><span class="sxs-lookup"><span data-stu-id="1a1e1-164">region</span></span>|<span data-ttu-id="1a1e1-165">string</span><span class="sxs-lookup"><span data-stu-id="1a1e1-165">string</span></span>| <span data-ttu-id="1a1e1-166">向其分配 connectorGroup 的区域并将为其优化流量。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-166">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="1a1e1-167">仅当未向 connectorGroup 分配 **连接器或应用程序** 时，才能设置此区域。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-167">This region can only be set if **no connectors or applications** are assigned to the connectorGroup.</span></span> <span data-ttu-id="1a1e1-168">可用区域包括：北美、欧洲、澳大利亚、亚洲和印度。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-168">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="1a1e1-169">可取值为：`nam`、`eur`、`aus`、`asia`、`ind`。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-169">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1e1-170">关系</span><span class="sxs-lookup"><span data-stu-id="1a1e1-170">Relationships</span></span>
| <span data-ttu-id="1a1e1-171">关系</span><span class="sxs-lookup"><span data-stu-id="1a1e1-171">Relationship</span></span> | <span data-ttu-id="1a1e1-172">类型</span><span class="sxs-lookup"><span data-stu-id="1a1e1-172">Type</span></span>   |<span data-ttu-id="1a1e1-173">说明</span><span class="sxs-lookup"><span data-stu-id="1a1e1-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1e1-174">来说</span><span class="sxs-lookup"><span data-stu-id="1a1e1-174">applications</span></span>|<span data-ttu-id="1a1e1-175">[application](application.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a1e1-175">[application](application.md) collection</span></span>| <span data-ttu-id="1a1e1-176">只读。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-176">Read-only.</span></span> <span data-ttu-id="1a1e1-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-177">Nullable.</span></span>|
|<span data-ttu-id="1a1e1-178">members</span><span class="sxs-lookup"><span data-stu-id="1a1e1-178">members</span></span>|<span data-ttu-id="1a1e1-179">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a1e1-179">[connector](connector.md) collection</span></span>| <span data-ttu-id="1a1e1-p109">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-p109">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a1e1-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a1e1-182">JSON representation</span></span>

<span data-ttu-id="1a1e1-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a1e1-183">The following is a JSON representation of the resource.</span></span>

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


