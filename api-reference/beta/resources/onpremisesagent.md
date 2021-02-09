---
title: onPremisesAgent 资源类型
description: onPremisesAgent 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 59ee11bb952c85695b8c20daa1e040c8899740b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158350"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="01c91-103">onPremisesAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="01c91-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="01c91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01c91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01c91-105">表示本地代理。</span><span class="sxs-lookup"><span data-stu-id="01c91-105">Represents on-premises agent.</span></span> <span data-ttu-id="01c91-106">租户管理员安装本地代理可以配置为访问/处理对特定已发布 [资源的请求](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="01c91-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="01c91-107">方法</span><span class="sxs-lookup"><span data-stu-id="01c91-107">Methods</span></span>

| <span data-ttu-id="01c91-108">方法</span><span class="sxs-lookup"><span data-stu-id="01c91-108">Method</span></span>       | <span data-ttu-id="01c91-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="01c91-109">Return Type</span></span> | <span data-ttu-id="01c91-110">说明</span><span class="sxs-lookup"><span data-stu-id="01c91-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="01c91-111">列出 onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="01c91-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="01c91-112">[onPremisesAgent](onpremisesagent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01c91-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="01c91-113">获取 **onPremisesAgents** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="01c91-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="01c91-114">获取 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="01c91-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="01c91-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="01c91-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="01c91-116">读取 **onPremisesAgent** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01c91-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="01c91-117">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="01c91-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="01c91-118">无</span><span class="sxs-lookup"><span data-stu-id="01c91-118">None</span></span> | <span data-ttu-id="01c91-119">将 **onPremisesAgent** 分配给 **onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="01c91-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="01c91-120">从 onPremisesAgentGroup 中删除 onpremisesAgent</span><span class="sxs-lookup"><span data-stu-id="01c91-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="01c91-121">无</span><span class="sxs-lookup"><span data-stu-id="01c91-121">None</span></span> | <span data-ttu-id="01c91-122">从 **onPremisesAgentGroup** 中删除 **onPremisesAgent**。</span><span class="sxs-lookup"><span data-stu-id="01c91-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="01c91-123">属性</span><span class="sxs-lookup"><span data-stu-id="01c91-123">Properties</span></span>

| <span data-ttu-id="01c91-124">属性</span><span class="sxs-lookup"><span data-stu-id="01c91-124">Property</span></span>     | <span data-ttu-id="01c91-125">类型</span><span class="sxs-lookup"><span data-stu-id="01c91-125">Type</span></span>        | <span data-ttu-id="01c91-126">说明</span><span class="sxs-lookup"><span data-stu-id="01c91-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01c91-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="01c91-127">externalIp</span></span>|<span data-ttu-id="01c91-128">String</span><span class="sxs-lookup"><span data-stu-id="01c91-128">String</span></span>|<span data-ttu-id="01c91-129">代理计算机的服务检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="01c91-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="01c91-130">只读</span><span class="sxs-lookup"><span data-stu-id="01c91-130">Read-only</span></span>|
|<span data-ttu-id="01c91-131">id</span><span class="sxs-lookup"><span data-stu-id="01c91-131">id</span></span>|<span data-ttu-id="01c91-132">String</span><span class="sxs-lookup"><span data-stu-id="01c91-132">String</span></span>| <span data-ttu-id="01c91-133">onPremisesAgent 的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="01c91-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="01c91-134">只读。</span><span class="sxs-lookup"><span data-stu-id="01c91-134">Read-only.</span></span>|
|<span data-ttu-id="01c91-135">machineName</span><span class="sxs-lookup"><span data-stu-id="01c91-135">machineName</span></span>|<span data-ttu-id="01c91-136">String</span><span class="sxs-lookup"><span data-stu-id="01c91-136">String</span></span>|<span data-ttu-id="01c91-137">正在运行的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="01c91-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="01c91-138">只读</span><span class="sxs-lookup"><span data-stu-id="01c91-138">Read-only</span></span>|
|<span data-ttu-id="01c91-139">状态</span><span class="sxs-lookup"><span data-stu-id="01c91-139">status</span></span>|<span data-ttu-id="01c91-140">string</span><span class="sxs-lookup"><span data-stu-id="01c91-140">string</span></span>| <span data-ttu-id="01c91-141">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="01c91-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="01c91-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="01c91-142">publishingType</span></span>|<span data-ttu-id="01c91-143">string</span><span class="sxs-lookup"><span data-stu-id="01c91-143">string</span></span>| <span data-ttu-id="01c91-144">可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="01c91-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01c91-145">关系</span><span class="sxs-lookup"><span data-stu-id="01c91-145">Relationships</span></span>

| <span data-ttu-id="01c91-146">关系</span><span class="sxs-lookup"><span data-stu-id="01c91-146">Relationship</span></span> | <span data-ttu-id="01c91-147">类型</span><span class="sxs-lookup"><span data-stu-id="01c91-147">Type</span></span>        | <span data-ttu-id="01c91-148">说明</span><span class="sxs-lookup"><span data-stu-id="01c91-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01c91-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="01c91-149">agentGroups</span></span>|<span data-ttu-id="01c91-150">[onPremisesAgentGroup](onpremisesagentgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01c91-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="01c91-151">**onPremisesAgent 分配到** 的 **onPremisesAgentGroups** 列表。</span><span class="sxs-lookup"><span data-stu-id="01c91-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="01c91-152">只读。</span><span class="sxs-lookup"><span data-stu-id="01c91-152">Read-only.</span></span> <span data-ttu-id="01c91-153">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="01c91-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01c91-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01c91-154">JSON representation</span></span>

<span data-ttu-id="01c91-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01c91-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



