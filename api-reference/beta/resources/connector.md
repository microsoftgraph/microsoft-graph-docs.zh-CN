---
title: 连接器资源类型
description: 表示应用程序代理连接器。
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e42bc42c1989e530f7b7f307da3963407ded112
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027165"
---
# <a name="connector-resource-type"></a><span data-ttu-id="1a0dd-103">连接器资源类型</span><span class="sxs-lookup"><span data-stu-id="1a0dd-103">connector resource type</span></span>

<span data-ttu-id="1a0dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a0dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a0dd-105">连接器是位于本地的轻型代理，便于与 [AZURE AD 应用程序代理](https://aka.ms/whyappproxy) 服务的出站连接。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="1a0dd-106">每个连接器都是 [connectorGroup](connectorgroup.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1a0dd-107">方法</span><span class="sxs-lookup"><span data-stu-id="1a0dd-107">Methods</span></span>

| <span data-ttu-id="1a0dd-108">方法</span><span class="sxs-lookup"><span data-stu-id="1a0dd-108">Method</span></span>       | <span data-ttu-id="1a0dd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a0dd-109">Return Type</span></span> | <span data-ttu-id="1a0dd-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a0dd-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1a0dd-111">List connectors</span><span class="sxs-lookup"><span data-stu-id="1a0dd-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="1a0dd-112">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a0dd-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="1a0dd-113">检索连接器对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="1a0dd-114">Get connector</span><span class="sxs-lookup"><span data-stu-id="1a0dd-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="1a0dd-115">连接器</span><span class="sxs-lookup"><span data-stu-id="1a0dd-115">connector</span></span>](connector.md) | <span data-ttu-id="1a0dd-116">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="1a0dd-117">List memberOf</span><span class="sxs-lookup"><span data-stu-id="1a0dd-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="1a0dd-118">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a0dd-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="1a0dd-119">列出连接器所属的 connectorGroup 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="1a0dd-120">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a0dd-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="1a0dd-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1a0dd-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="1a0dd-122">将连接器添加到 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="1a0dd-123">属性</span><span class="sxs-lookup"><span data-stu-id="1a0dd-123">Properties</span></span>
| <span data-ttu-id="1a0dd-124">属性</span><span class="sxs-lookup"><span data-stu-id="1a0dd-124">Property</span></span>     | <span data-ttu-id="1a0dd-125">类型</span><span class="sxs-lookup"><span data-stu-id="1a0dd-125">Type</span></span>        | <span data-ttu-id="1a0dd-126">说明</span><span class="sxs-lookup"><span data-stu-id="1a0dd-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a0dd-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="1a0dd-127">externalIp</span></span>|<span data-ttu-id="1a0dd-128">String</span><span class="sxs-lookup"><span data-stu-id="1a0dd-128">String</span></span>| <span data-ttu-id="1a0dd-129">连接器服务器检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="1a0dd-130">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-130">Read-only.</span></span> |
|<span data-ttu-id="1a0dd-131">id</span><span class="sxs-lookup"><span data-stu-id="1a0dd-131">id</span></span>|<span data-ttu-id="1a0dd-132">String</span><span class="sxs-lookup"><span data-stu-id="1a0dd-132">String</span></span>| <span data-ttu-id="1a0dd-133">连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-133">Unique identifier of the connector.</span></span> <span data-ttu-id="1a0dd-134">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-134">Read-only.</span></span> |
|<span data-ttu-id="1a0dd-135">machineName</span><span class="sxs-lookup"><span data-stu-id="1a0dd-135">machineName</span></span>|<span data-ttu-id="1a0dd-136">String</span><span class="sxs-lookup"><span data-stu-id="1a0dd-136">String</span></span>| <span data-ttu-id="1a0dd-137">连接器已安装并在其上运行的计算机名称。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="1a0dd-138">状态</span><span class="sxs-lookup"><span data-stu-id="1a0dd-138">status</span></span>|<span data-ttu-id="1a0dd-139">string</span><span class="sxs-lookup"><span data-stu-id="1a0dd-139">string</span></span>| <span data-ttu-id="1a0dd-140">指示连接器的状态。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-140">Indicates the status of the connector.</span></span> <span data-ttu-id="1a0dd-141">可能的值是：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="1a0dd-142">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1a0dd-143">关系</span><span class="sxs-lookup"><span data-stu-id="1a0dd-143">Relationships</span></span>
| <span data-ttu-id="1a0dd-144">关系</span><span class="sxs-lookup"><span data-stu-id="1a0dd-144">Relationship</span></span> | <span data-ttu-id="1a0dd-145">类型</span><span class="sxs-lookup"><span data-stu-id="1a0dd-145">Type</span></span>   |<span data-ttu-id="1a0dd-146">说明</span><span class="sxs-lookup"><span data-stu-id="1a0dd-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a0dd-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="1a0dd-147">memberOf</span></span>|<span data-ttu-id="1a0dd-148">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a0dd-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="1a0dd-149">连接器所属的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="1a0dd-150">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1a0dd-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a0dd-151">JSON representation</span></span>

<span data-ttu-id="1a0dd-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a0dd-152">The following is a JSON representation of the resource.</span></span>

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


