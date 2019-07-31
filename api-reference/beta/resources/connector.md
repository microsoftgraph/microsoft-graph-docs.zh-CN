---
title: 连接器资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec4d3fdb415533d5b3f2effc72688fe912551bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012875"
---
# <a name="connector-resource-type"></a><span data-ttu-id="3f31c-103">连接器资源类型</span><span class="sxs-lookup"><span data-stu-id="3f31c-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="3f31c-104">方法</span><span class="sxs-lookup"><span data-stu-id="3f31c-104">Methods</span></span>

| <span data-ttu-id="3f31c-105">方法</span><span class="sxs-lookup"><span data-stu-id="3f31c-105">Method</span></span>           | <span data-ttu-id="3f31c-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f31c-106">Return Type</span></span>    |<span data-ttu-id="3f31c-107">说明</span><span class="sxs-lookup"><span data-stu-id="3f31c-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f31c-108">获取连接器</span><span class="sxs-lookup"><span data-stu-id="3f31c-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="3f31c-109">连接器</span><span class="sxs-lookup"><span data-stu-id="3f31c-109">connector</span></span>](connector.md) |<span data-ttu-id="3f31c-110">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f31c-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="3f31c-111">List memberOf</span><span class="sxs-lookup"><span data-stu-id="3f31c-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="3f31c-112">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f31c-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="3f31c-113">获取与连接器关联的 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="3f31c-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f31c-114">属性</span><span class="sxs-lookup"><span data-stu-id="3f31c-114">Properties</span></span>
| <span data-ttu-id="3f31c-115">属性</span><span class="sxs-lookup"><span data-stu-id="3f31c-115">Property</span></span>     | <span data-ttu-id="3f31c-116">类型</span><span class="sxs-lookup"><span data-stu-id="3f31c-116">Type</span></span>   |<span data-ttu-id="3f31c-117">说明</span><span class="sxs-lookup"><span data-stu-id="3f31c-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f31c-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="3f31c-118">externalIp</span></span>|<span data-ttu-id="3f31c-119">String</span><span class="sxs-lookup"><span data-stu-id="3f31c-119">String</span></span>|<span data-ttu-id="3f31c-120">由连接器计算机的服务检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="3f31c-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="3f31c-121">只读</span><span class="sxs-lookup"><span data-stu-id="3f31c-121">Read-only</span></span>|
|<span data-ttu-id="3f31c-122">id</span><span class="sxs-lookup"><span data-stu-id="3f31c-122">id</span></span>|<span data-ttu-id="3f31c-123">String</span><span class="sxs-lookup"><span data-stu-id="3f31c-123">String</span></span>| <span data-ttu-id="3f31c-124">连接器的对象 id。</span><span class="sxs-lookup"><span data-stu-id="3f31c-124">The object id of the connector.</span></span> <BR><span data-ttu-id="3f31c-125">只读。</span><span class="sxs-lookup"><span data-stu-id="3f31c-125">Read-only.</span></span>|
|<span data-ttu-id="3f31c-126">machineName</span><span class="sxs-lookup"><span data-stu-id="3f31c-126">machineName</span></span>|<span data-ttu-id="3f31c-127">String</span><span class="sxs-lookup"><span data-stu-id="3f31c-127">String</span></span>| <span data-ttu-id="3f31c-128">运行连接器的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="3f31c-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="3f31c-129">只读</span><span class="sxs-lookup"><span data-stu-id="3f31c-129">Read-only</span></span>|
|<span data-ttu-id="3f31c-130">状态</span><span class="sxs-lookup"><span data-stu-id="3f31c-130">status</span></span>|<span data-ttu-id="3f31c-131">string</span><span class="sxs-lookup"><span data-stu-id="3f31c-131">string</span></span>| <span data-ttu-id="3f31c-132">指示连接器的状态。</span><span class="sxs-lookup"><span data-stu-id="3f31c-132">Indicates the status of the connector.</span></span> <span data-ttu-id="3f31c-133">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="3f31c-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="3f31c-134">只读</span><span class="sxs-lookup"><span data-stu-id="3f31c-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="3f31c-135">关系</span><span class="sxs-lookup"><span data-stu-id="3f31c-135">Relationships</span></span>
| <span data-ttu-id="3f31c-136">关系</span><span class="sxs-lookup"><span data-stu-id="3f31c-136">Relationship</span></span> | <span data-ttu-id="3f31c-137">类型</span><span class="sxs-lookup"><span data-stu-id="3f31c-137">Type</span></span>   |<span data-ttu-id="3f31c-138">说明</span><span class="sxs-lookup"><span data-stu-id="3f31c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f31c-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="3f31c-139">memberOf</span></span>|<span data-ttu-id="3f31c-140">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f31c-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="3f31c-141">连接是其成员的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="3f31c-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="3f31c-142">只读。</span><span class="sxs-lookup"><span data-stu-id="3f31c-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3f31c-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f31c-143">JSON representation</span></span>

<span data-ttu-id="3f31c-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f31c-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
