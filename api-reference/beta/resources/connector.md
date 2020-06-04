---
title: 连接器资源类型
description: 表示应用程序代理连接器。
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864d76d7e6a7cb3724a91a753e5c5198e274780a
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556175"
---
# <a name="connector-resource-type"></a><span data-ttu-id="5c611-103">连接器资源类型</span><span class="sxs-lookup"><span data-stu-id="5c611-103">connector resource type</span></span>

<span data-ttu-id="5c611-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c611-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c611-105">连接器是位于本地的轻型代理，便于与[AZURE AD 应用程序代理](https://aka.ms/whyappproxy)服务的出站连接。</span><span class="sxs-lookup"><span data-stu-id="5c611-105">Connectors are lightweight agents that sit on-premises and facilitate the outbound connection to the [Azure AD Application Proxy](https://aka.ms/whyappproxy) service.</span></span> <span data-ttu-id="5c611-106">每个连接器都是[connectorGroup](connectorgroup.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="5c611-106">Each connector is part of a [connectorGroup](connectorgroup.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5c611-107">Methods</span><span class="sxs-lookup"><span data-stu-id="5c611-107">Methods</span></span>

| <span data-ttu-id="5c611-108">方法</span><span class="sxs-lookup"><span data-stu-id="5c611-108">Method</span></span>       | <span data-ttu-id="5c611-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c611-109">Return Type</span></span> | <span data-ttu-id="5c611-110">说明</span><span class="sxs-lookup"><span data-stu-id="5c611-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5c611-111">列出连接器</span><span class="sxs-lookup"><span data-stu-id="5c611-111">List connectors</span></span>](../api/connector-list.md) | <span data-ttu-id="5c611-112">[连接器](connector.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c611-112">[connector](connector.md) collection</span></span> | <span data-ttu-id="5c611-113">检索连接器对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5c611-113">Retrieve a list of connector objects.</span></span> | 
| [<span data-ttu-id="5c611-114">获取连接器</span><span class="sxs-lookup"><span data-stu-id="5c611-114">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="5c611-115">连接器</span><span class="sxs-lookup"><span data-stu-id="5c611-115">connector</span></span>](connector.md) | <span data-ttu-id="5c611-116">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c611-116">Read properties and relationships of connector object.</span></span> |
| [<span data-ttu-id="5c611-117">List memberOf</span><span class="sxs-lookup"><span data-stu-id="5c611-117">List memberOf</span></span>](../api/connector-list-memberof.md) | <span data-ttu-id="5c611-118">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c611-118">[connectorGroup](connectorgroup.md) collection</span></span> | <span data-ttu-id="5c611-119">列出连接器所属的 connectorGroup 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5c611-119">List the connectorGroup object collection the connector is a member of.</span></span> |
| [<span data-ttu-id="5c611-120">将连接器添加到 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c611-120">Add connector to connectorGroup</span></span>](../api/connector-post-memberof.md)| [<span data-ttu-id="5c611-121">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="5c611-121">connectorGroup</span></span>](connectorgroup.md) | <span data-ttu-id="5c611-122">将连接器添加到 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="5c611-122">Add a connector to a connectorGroup.</span></span> |


## <a name="properties"></a><span data-ttu-id="5c611-123">属性</span><span class="sxs-lookup"><span data-stu-id="5c611-123">Properties</span></span>
| <span data-ttu-id="5c611-124">属性</span><span class="sxs-lookup"><span data-stu-id="5c611-124">Property</span></span>     | <span data-ttu-id="5c611-125">类型</span><span class="sxs-lookup"><span data-stu-id="5c611-125">Type</span></span>        | <span data-ttu-id="5c611-126">说明</span><span class="sxs-lookup"><span data-stu-id="5c611-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c611-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="5c611-127">externalIp</span></span>|<span data-ttu-id="5c611-128">String</span><span class="sxs-lookup"><span data-stu-id="5c611-128">String</span></span>| <span data-ttu-id="5c611-129">连接器服务器检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="5c611-129">The external IP address as detected by the the connector server.</span></span> <span data-ttu-id="5c611-130">只读。</span><span class="sxs-lookup"><span data-stu-id="5c611-130">Read-only.</span></span> |
|<span data-ttu-id="5c611-131">id</span><span class="sxs-lookup"><span data-stu-id="5c611-131">id</span></span>|<span data-ttu-id="5c611-132">String</span><span class="sxs-lookup"><span data-stu-id="5c611-132">String</span></span>| <span data-ttu-id="5c611-133">连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5c611-133">Unique identifier of the connector.</span></span> <span data-ttu-id="5c611-134">只读。</span><span class="sxs-lookup"><span data-stu-id="5c611-134">Read-only.</span></span> |
|<span data-ttu-id="5c611-135">machineName</span><span class="sxs-lookup"><span data-stu-id="5c611-135">machineName</span></span>|<span data-ttu-id="5c611-136">String</span><span class="sxs-lookup"><span data-stu-id="5c611-136">String</span></span>| <span data-ttu-id="5c611-137">连接器已安装并在其上运行的计算机名称。</span><span class="sxs-lookup"><span data-stu-id="5c611-137">The machine name the connector is installed and running on.</span></span> |
|<span data-ttu-id="5c611-138">状态</span><span class="sxs-lookup"><span data-stu-id="5c611-138">status</span></span>|<span data-ttu-id="5c611-139">string</span><span class="sxs-lookup"><span data-stu-id="5c611-139">string</span></span>| <span data-ttu-id="5c611-140">指示连接器的状态。</span><span class="sxs-lookup"><span data-stu-id="5c611-140">Indicates the status of the connector.</span></span> <span data-ttu-id="5c611-141">可能的值是：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="5c611-141">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="5c611-142">只读。</span><span class="sxs-lookup"><span data-stu-id="5c611-142">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5c611-143">关系</span><span class="sxs-lookup"><span data-stu-id="5c611-143">Relationships</span></span>
| <span data-ttu-id="5c611-144">关系</span><span class="sxs-lookup"><span data-stu-id="5c611-144">Relationship</span></span> | <span data-ttu-id="5c611-145">类型</span><span class="sxs-lookup"><span data-stu-id="5c611-145">Type</span></span>   |<span data-ttu-id="5c611-146">说明</span><span class="sxs-lookup"><span data-stu-id="5c611-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c611-147">memberOf</span><span class="sxs-lookup"><span data-stu-id="5c611-147">memberOf</span></span>|<span data-ttu-id="5c611-148">[connectorGroup](connectorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c611-148">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="5c611-149">连接器所属的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="5c611-149">The connectorGroup that the connector is a member of.</span></span> <span data-ttu-id="5c611-150">只读。</span><span class="sxs-lookup"><span data-stu-id="5c611-150">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c611-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c611-151">JSON representation</span></span>

<span data-ttu-id="5c611-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c611-152">The following is a JSON representation of the resource.</span></span>

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
