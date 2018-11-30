---
title: 连接器资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047930"
---
# <a name="connector-resource-type"></a><span data-ttu-id="932dc-103">连接器资源类型</span><span class="sxs-lookup"><span data-stu-id="932dc-103">connector resource type</span></span>

> <span data-ttu-id="932dc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="932dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="932dc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="932dc-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="932dc-106">方法</span><span class="sxs-lookup"><span data-stu-id="932dc-106">Methods</span></span>

| <span data-ttu-id="932dc-107">方法</span><span class="sxs-lookup"><span data-stu-id="932dc-107">Method</span></span>           | <span data-ttu-id="932dc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="932dc-108">Return Type</span></span>    |<span data-ttu-id="932dc-109">说明</span><span class="sxs-lookup"><span data-stu-id="932dc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="932dc-110">获取连接器</span><span class="sxs-lookup"><span data-stu-id="932dc-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="932dc-111">连接器</span><span class="sxs-lookup"><span data-stu-id="932dc-111">connector</span></span>](connector.md) |<span data-ttu-id="932dc-112">读取属性和连接器对象的关系。</span><span class="sxs-lookup"><span data-stu-id="932dc-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="932dc-113">List memberOf</span><span class="sxs-lookup"><span data-stu-id="932dc-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="932dc-114">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="932dc-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="932dc-115">获取与连接器相关联的 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="932dc-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="932dc-116">属性</span><span class="sxs-lookup"><span data-stu-id="932dc-116">Properties</span></span>
| <span data-ttu-id="932dc-117">属性</span><span class="sxs-lookup"><span data-stu-id="932dc-117">Property</span></span>     | <span data-ttu-id="932dc-118">类型</span><span class="sxs-lookup"><span data-stu-id="932dc-118">Type</span></span>   |<span data-ttu-id="932dc-119">说明</span><span class="sxs-lookup"><span data-stu-id="932dc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="932dc-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="932dc-120">externalIp</span></span>|<span data-ttu-id="932dc-121">字符串</span><span class="sxs-lookup"><span data-stu-id="932dc-121">String</span></span>|<span data-ttu-id="932dc-122">作为服务为连接器计算机检测到外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="932dc-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="932dc-123">只读</span><span class="sxs-lookup"><span data-stu-id="932dc-123">Read-only</span></span>|
|<span data-ttu-id="932dc-124">id</span><span class="sxs-lookup"><span data-stu-id="932dc-124">id</span></span>|<span data-ttu-id="932dc-125">字符串</span><span class="sxs-lookup"><span data-stu-id="932dc-125">String</span></span>| <span data-ttu-id="932dc-126">连接符的对象 id。</span><span class="sxs-lookup"><span data-stu-id="932dc-126">The object id of the connector.</span></span> <BR><span data-ttu-id="932dc-127">只读。</span><span class="sxs-lookup"><span data-stu-id="932dc-127">Read-only.</span></span>|
|<span data-ttu-id="932dc-128">计算机名</span><span class="sxs-lookup"><span data-stu-id="932dc-128">machineName</span></span>|<span data-ttu-id="932dc-129">字符串</span><span class="sxs-lookup"><span data-stu-id="932dc-129">String</span></span>| <span data-ttu-id="932dc-130">运行连接器的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="932dc-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="932dc-131">只读</span><span class="sxs-lookup"><span data-stu-id="932dc-131">Read-only</span></span>|
|<span data-ttu-id="932dc-132">status</span><span class="sxs-lookup"><span data-stu-id="932dc-132">status</span></span>|<span data-ttu-id="932dc-133">string</span><span class="sxs-lookup"><span data-stu-id="932dc-133">string</span></span>| <span data-ttu-id="932dc-134">指示连接符的状态。</span><span class="sxs-lookup"><span data-stu-id="932dc-134">Indicates the status of the connector.</span></span> <span data-ttu-id="932dc-135">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="932dc-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="932dc-136">只读</span><span class="sxs-lookup"><span data-stu-id="932dc-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="932dc-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="932dc-137">Relationships</span></span>
| <span data-ttu-id="932dc-138">关系</span><span class="sxs-lookup"><span data-stu-id="932dc-138">Relationship</span></span> | <span data-ttu-id="932dc-139">类型</span><span class="sxs-lookup"><span data-stu-id="932dc-139">Type</span></span>   |<span data-ttu-id="932dc-140">说明</span><span class="sxs-lookup"><span data-stu-id="932dc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="932dc-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="932dc-141">memberOf</span></span>|<span data-ttu-id="932dc-142">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="932dc-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="932dc-143">ConnectorGroup 的连接的成员。</span><span class="sxs-lookup"><span data-stu-id="932dc-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="932dc-144">只读。</span><span class="sxs-lookup"><span data-stu-id="932dc-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="932dc-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="932dc-145">JSON representation</span></span>

<span data-ttu-id="932dc-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="932dc-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
