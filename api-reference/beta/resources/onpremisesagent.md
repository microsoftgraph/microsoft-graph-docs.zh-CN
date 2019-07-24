---
title: onPremisesAgent 资源类型
description: onPremisesAgent 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bcff659cf30b946654f14190b2cf5f693d27bc4
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841260"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="87c69-103">onPremisesAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="87c69-103">onPremisesAgent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c69-104">表示内部部署代理。</span><span class="sxs-lookup"><span data-stu-id="87c69-104">Represents on-premises agent.</span></span> <span data-ttu-id="87c69-105">可将租户管理员安装的本地代理配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="87c69-105">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="87c69-106">方法</span><span class="sxs-lookup"><span data-stu-id="87c69-106">Methods</span></span>

| <span data-ttu-id="87c69-107">方法</span><span class="sxs-lookup"><span data-stu-id="87c69-107">Method</span></span>       | <span data-ttu-id="87c69-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="87c69-108">Return Type</span></span> | <span data-ttu-id="87c69-109">说明</span><span class="sxs-lookup"><span data-stu-id="87c69-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="87c69-110">列出 onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="87c69-110">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="87c69-111">[onPremisesAgent](onpremisesagent.md)集合</span><span class="sxs-lookup"><span data-stu-id="87c69-111">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="87c69-112">获取**onPremisesAgents**对象集合。</span><span class="sxs-lookup"><span data-stu-id="87c69-112">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="87c69-113">获取 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="87c69-113">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="87c69-114">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="87c69-114">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="87c69-115">读取**onPremisesAgent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87c69-115">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="87c69-116">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="87c69-116">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="87c69-117">无</span><span class="sxs-lookup"><span data-stu-id="87c69-117">None</span></span> | <span data-ttu-id="87c69-118">将**onPremisesAgent**分配给**onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="87c69-118">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="87c69-119">从 onPremisesAgentGroup 中删除 onpremisesAgent</span><span class="sxs-lookup"><span data-stu-id="87c69-119">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="87c69-120">无</span><span class="sxs-lookup"><span data-stu-id="87c69-120">None</span></span> | <span data-ttu-id="87c69-121">从**onPremisesAgentGroup**中删除**onPremisesAgent** 。</span><span class="sxs-lookup"><span data-stu-id="87c69-121">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="87c69-122">属性</span><span class="sxs-lookup"><span data-stu-id="87c69-122">Properties</span></span>

| <span data-ttu-id="87c69-123">属性</span><span class="sxs-lookup"><span data-stu-id="87c69-123">Property</span></span>     | <span data-ttu-id="87c69-124">类型</span><span class="sxs-lookup"><span data-stu-id="87c69-124">Type</span></span>        | <span data-ttu-id="87c69-125">说明</span><span class="sxs-lookup"><span data-stu-id="87c69-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87c69-126">externalIp</span><span class="sxs-lookup"><span data-stu-id="87c69-126">externalIp</span></span>|<span data-ttu-id="87c69-127">String</span><span class="sxs-lookup"><span data-stu-id="87c69-127">String</span></span>|<span data-ttu-id="87c69-128">由代理计算机的服务检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="87c69-128">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="87c69-129">只读</span><span class="sxs-lookup"><span data-stu-id="87c69-129">Read-only</span></span>|
|<span data-ttu-id="87c69-130">id</span><span class="sxs-lookup"><span data-stu-id="87c69-130">id</span></span>|<span data-ttu-id="87c69-131">String</span><span class="sxs-lookup"><span data-stu-id="87c69-131">String</span></span>| <span data-ttu-id="87c69-132">OnPremisesAgent 的对象 id。</span><span class="sxs-lookup"><span data-stu-id="87c69-132">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="87c69-133">只读。</span><span class="sxs-lookup"><span data-stu-id="87c69-133">Read-only.</span></span>|
|<span data-ttu-id="87c69-134">machineName</span><span class="sxs-lookup"><span data-stu-id="87c69-134">machineName</span></span>|<span data-ttu-id="87c69-135">String</span><span class="sxs-lookup"><span data-stu-id="87c69-135">String</span></span>|<span data-ttu-id="87c69-136">运行 aggent 的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="87c69-136">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="87c69-137">只读</span><span class="sxs-lookup"><span data-stu-id="87c69-137">Read-only</span></span>|
|<span data-ttu-id="87c69-138">状态</span><span class="sxs-lookup"><span data-stu-id="87c69-138">status</span></span>|<span data-ttu-id="87c69-139">string</span><span class="sxs-lookup"><span data-stu-id="87c69-139">string</span></span>| <span data-ttu-id="87c69-140">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="87c69-140">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="87c69-141">publishingType</span><span class="sxs-lookup"><span data-stu-id="87c69-141">publishingType</span></span>|<span data-ttu-id="87c69-142">string</span><span class="sxs-lookup"><span data-stu-id="87c69-142">string</span></span>| <span data-ttu-id="87c69-143">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="87c69-143">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87c69-144">关系</span><span class="sxs-lookup"><span data-stu-id="87c69-144">Relationships</span></span>

| <span data-ttu-id="87c69-145">关系</span><span class="sxs-lookup"><span data-stu-id="87c69-145">Relationship</span></span> | <span data-ttu-id="87c69-146">类型</span><span class="sxs-lookup"><span data-stu-id="87c69-146">Type</span></span>        | <span data-ttu-id="87c69-147">说明</span><span class="sxs-lookup"><span data-stu-id="87c69-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87c69-148">agentGroups</span><span class="sxs-lookup"><span data-stu-id="87c69-148">agentGroups</span></span>|<span data-ttu-id="87c69-149">[onPremisesAgentGroup](onpremisesagentgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="87c69-149">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="87c69-150">向其分配**onPremisesAgent**的**onPremisesAgentGroups**的列表。</span><span class="sxs-lookup"><span data-stu-id="87c69-150">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="87c69-151">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="87c69-151">Read-only.</span></span> <span data-ttu-id="87c69-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="87c69-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87c69-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87c69-153">JSON representation</span></span>

<span data-ttu-id="87c69-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87c69-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
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
