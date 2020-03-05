---
title: 连接器资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25d350e48aaddbda2b931ae5a9e177ec6caa9799
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507476"
---
# <a name="connector-resource-type"></a><span data-ttu-id="4b822-103">连接器资源类型</span><span class="sxs-lookup"><span data-stu-id="4b822-103">connector resource type</span></span>

<span data-ttu-id="4b822-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4b822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="4b822-105">方法</span><span class="sxs-lookup"><span data-stu-id="4b822-105">Methods</span></span>

| <span data-ttu-id="4b822-106">方法</span><span class="sxs-lookup"><span data-stu-id="4b822-106">Method</span></span>           | <span data-ttu-id="4b822-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b822-107">Return Type</span></span>    |<span data-ttu-id="4b822-108">说明</span><span class="sxs-lookup"><span data-stu-id="4b822-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b822-109">获取连接器</span><span class="sxs-lookup"><span data-stu-id="4b822-109">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="4b822-110">连接器</span><span class="sxs-lookup"><span data-stu-id="4b822-110">connector</span></span>](connector.md) |<span data-ttu-id="4b822-111">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b822-111">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="4b822-112">List memberOf</span><span class="sxs-lookup"><span data-stu-id="4b822-112">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="4b822-113">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b822-113">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="4b822-114">获取与连接器关联的 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="4b822-114">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b822-115">属性</span><span class="sxs-lookup"><span data-stu-id="4b822-115">Properties</span></span>
| <span data-ttu-id="4b822-116">属性</span><span class="sxs-lookup"><span data-stu-id="4b822-116">Property</span></span>     | <span data-ttu-id="4b822-117">类型</span><span class="sxs-lookup"><span data-stu-id="4b822-117">Type</span></span>   |<span data-ttu-id="4b822-118">说明</span><span class="sxs-lookup"><span data-stu-id="4b822-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b822-119">externalIp</span><span class="sxs-lookup"><span data-stu-id="4b822-119">externalIp</span></span>|<span data-ttu-id="4b822-120">String</span><span class="sxs-lookup"><span data-stu-id="4b822-120">String</span></span>|<span data-ttu-id="4b822-121">由连接器计算机的服务检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="4b822-121">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="4b822-122">只读</span><span class="sxs-lookup"><span data-stu-id="4b822-122">Read-only</span></span>|
|<span data-ttu-id="4b822-123">id</span><span class="sxs-lookup"><span data-stu-id="4b822-123">id</span></span>|<span data-ttu-id="4b822-124">String</span><span class="sxs-lookup"><span data-stu-id="4b822-124">String</span></span>| <span data-ttu-id="4b822-125">连接器的对象 id。</span><span class="sxs-lookup"><span data-stu-id="4b822-125">The object id of the connector.</span></span> <BR><span data-ttu-id="4b822-126">只读。</span><span class="sxs-lookup"><span data-stu-id="4b822-126">Read-only.</span></span>|
|<span data-ttu-id="4b822-127">machineName</span><span class="sxs-lookup"><span data-stu-id="4b822-127">machineName</span></span>|<span data-ttu-id="4b822-128">String</span><span class="sxs-lookup"><span data-stu-id="4b822-128">String</span></span>| <span data-ttu-id="4b822-129">运行连接器的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="4b822-129">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="4b822-130">只读</span><span class="sxs-lookup"><span data-stu-id="4b822-130">Read-only</span></span>|
|<span data-ttu-id="4b822-131">状态</span><span class="sxs-lookup"><span data-stu-id="4b822-131">status</span></span>|<span data-ttu-id="4b822-132">string</span><span class="sxs-lookup"><span data-stu-id="4b822-132">string</span></span>| <span data-ttu-id="4b822-133">指示连接器的状态。</span><span class="sxs-lookup"><span data-stu-id="4b822-133">Indicates the status of the connector.</span></span> <span data-ttu-id="4b822-134">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="4b822-134">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="4b822-135">只读</span><span class="sxs-lookup"><span data-stu-id="4b822-135">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="4b822-136">关系</span><span class="sxs-lookup"><span data-stu-id="4b822-136">Relationships</span></span>
| <span data-ttu-id="4b822-137">关系</span><span class="sxs-lookup"><span data-stu-id="4b822-137">Relationship</span></span> | <span data-ttu-id="4b822-138">类型</span><span class="sxs-lookup"><span data-stu-id="4b822-138">Type</span></span>   |<span data-ttu-id="4b822-139">说明</span><span class="sxs-lookup"><span data-stu-id="4b822-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b822-140">memberOf</span><span class="sxs-lookup"><span data-stu-id="4b822-140">memberOf</span></span>|<span data-ttu-id="4b822-141">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b822-141">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="4b822-142">连接是其成员的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="4b822-142">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="4b822-143">只读。</span><span class="sxs-lookup"><span data-stu-id="4b822-143">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b822-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b822-144">JSON representation</span></span>

<span data-ttu-id="4b822-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b822-145">Here is a JSON representation of the resource.</span></span>

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
