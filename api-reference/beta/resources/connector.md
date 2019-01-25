---
title: 连接器资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525729"
---
# <a name="connector-resource-type"></a><span data-ttu-id="a1aa4-103">连接器资源类型</span><span class="sxs-lookup"><span data-stu-id="a1aa4-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="a1aa4-104">方法</span><span class="sxs-lookup"><span data-stu-id="a1aa4-104">Methods</span></span>

| <span data-ttu-id="a1aa4-105">方法</span><span class="sxs-lookup"><span data-stu-id="a1aa4-105">Method</span></span>           | <span data-ttu-id="a1aa4-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1aa4-106">Return Type</span></span>    |<span data-ttu-id="a1aa4-107">说明</span><span class="sxs-lookup"><span data-stu-id="a1aa4-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1aa4-108">获取连接器</span><span class="sxs-lookup"><span data-stu-id="a1aa4-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="a1aa4-109">Connector</span><span class="sxs-lookup"><span data-stu-id="a1aa4-109">connector</span></span>](connector.md) |<span data-ttu-id="a1aa4-110">读取属性和连接器对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="a1aa4-111">List memberOf</span><span class="sxs-lookup"><span data-stu-id="a1aa4-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="a1aa4-112">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="a1aa4-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="a1aa4-113">获取与连接器相关联的 connectorGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1aa4-114">属性</span><span class="sxs-lookup"><span data-stu-id="a1aa4-114">Properties</span></span>
| <span data-ttu-id="a1aa4-115">属性</span><span class="sxs-lookup"><span data-stu-id="a1aa4-115">Property</span></span>     | <span data-ttu-id="a1aa4-116">类型</span><span class="sxs-lookup"><span data-stu-id="a1aa4-116">Type</span></span>   |<span data-ttu-id="a1aa4-117">说明</span><span class="sxs-lookup"><span data-stu-id="a1aa4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1aa4-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="a1aa4-118">externalIp</span></span>|<span data-ttu-id="a1aa4-119">String</span><span class="sxs-lookup"><span data-stu-id="a1aa4-119">String</span></span>|<span data-ttu-id="a1aa4-120">作为服务为连接器计算机检测到外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="a1aa4-121">只读</span><span class="sxs-lookup"><span data-stu-id="a1aa4-121">Read-only</span></span>|
|<span data-ttu-id="a1aa4-122">id</span><span class="sxs-lookup"><span data-stu-id="a1aa4-122">id</span></span>|<span data-ttu-id="a1aa4-123">字串符号</span><span class="sxs-lookup"><span data-stu-id="a1aa4-123">String</span></span>| <span data-ttu-id="a1aa4-124">连接符的对象 id。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-124">The object id of the connector.</span></span> <BR><span data-ttu-id="a1aa4-125">只读。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-125">Read-only.</span></span>|
|<span data-ttu-id="a1aa4-126">计算机名</span><span class="sxs-lookup"><span data-stu-id="a1aa4-126">machineName</span></span>|<span data-ttu-id="a1aa4-127">String</span><span class="sxs-lookup"><span data-stu-id="a1aa4-127">String</span></span>| <span data-ttu-id="a1aa4-128">运行连接器的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="a1aa4-129">只读</span><span class="sxs-lookup"><span data-stu-id="a1aa4-129">Read-only</span></span>|
|<span data-ttu-id="a1aa4-130">status</span><span class="sxs-lookup"><span data-stu-id="a1aa4-130">status</span></span>|<span data-ttu-id="a1aa4-131">string</span><span class="sxs-lookup"><span data-stu-id="a1aa4-131">string</span></span>| <span data-ttu-id="a1aa4-132">指示连接符的状态。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-132">Indicates the status of the connector.</span></span> <span data-ttu-id="a1aa4-133">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="a1aa4-134">只读</span><span class="sxs-lookup"><span data-stu-id="a1aa4-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="a1aa4-135">关系</span><span class="sxs-lookup"><span data-stu-id="a1aa4-135">Relationships</span></span>
| <span data-ttu-id="a1aa4-136">关系</span><span class="sxs-lookup"><span data-stu-id="a1aa4-136">Relationship</span></span> | <span data-ttu-id="a1aa4-137">类型</span><span class="sxs-lookup"><span data-stu-id="a1aa4-137">Type</span></span>   |<span data-ttu-id="a1aa4-138">说明</span><span class="sxs-lookup"><span data-stu-id="a1aa4-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1aa4-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="a1aa4-139">memberOf</span></span>|<span data-ttu-id="a1aa4-140">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="a1aa4-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="a1aa4-141">ConnectorGroup 的连接的成员。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="a1aa4-142">只读。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1aa4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1aa4-143">JSON representation</span></span>

<span data-ttu-id="a1aa4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1aa4-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
