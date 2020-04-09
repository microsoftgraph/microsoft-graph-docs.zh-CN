---
title: onPremisesAgent 资源类型
description: onPremisesAgent 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fdc6355b33539899ab51a4a6881a8109cb8d87a6
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199751"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="a971f-103">onPremisesAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a971f-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="a971f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a971f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a971f-105">表示内部部署代理。</span><span class="sxs-lookup"><span data-stu-id="a971f-105">Represents on-premises agent.</span></span> <span data-ttu-id="a971f-106">可将租户管理员安装的本地代理配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="a971f-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a971f-107">方法</span><span class="sxs-lookup"><span data-stu-id="a971f-107">Methods</span></span>

| <span data-ttu-id="a971f-108">方法</span><span class="sxs-lookup"><span data-stu-id="a971f-108">Method</span></span>       | <span data-ttu-id="a971f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a971f-109">Return Type</span></span> | <span data-ttu-id="a971f-110">说明</span><span class="sxs-lookup"><span data-stu-id="a971f-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a971f-111">列出 onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="a971f-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="a971f-112">[onPremisesAgent](onpremisesagent.md)集合</span><span class="sxs-lookup"><span data-stu-id="a971f-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="a971f-113">获取**onPremisesAgents**对象集合。</span><span class="sxs-lookup"><span data-stu-id="a971f-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="a971f-114">获取 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="a971f-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="a971f-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="a971f-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="a971f-116">读取**onPremisesAgent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a971f-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="a971f-117">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="a971f-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="a971f-118">无</span><span class="sxs-lookup"><span data-stu-id="a971f-118">None</span></span> | <span data-ttu-id="a971f-119">将**onPremisesAgent**分配给**onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="a971f-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="a971f-120">从 onPremisesAgentGroup 中删除 onpremisesAgent</span><span class="sxs-lookup"><span data-stu-id="a971f-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="a971f-121">无</span><span class="sxs-lookup"><span data-stu-id="a971f-121">None</span></span> | <span data-ttu-id="a971f-122">从**onPremisesAgentGroup**中删除**onPremisesAgent** 。</span><span class="sxs-lookup"><span data-stu-id="a971f-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="a971f-123">属性</span><span class="sxs-lookup"><span data-stu-id="a971f-123">Properties</span></span>

| <span data-ttu-id="a971f-124">属性</span><span class="sxs-lookup"><span data-stu-id="a971f-124">Property</span></span>     | <span data-ttu-id="a971f-125">类型</span><span class="sxs-lookup"><span data-stu-id="a971f-125">Type</span></span>        | <span data-ttu-id="a971f-126">说明</span><span class="sxs-lookup"><span data-stu-id="a971f-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a971f-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="a971f-127">externalIp</span></span>|<span data-ttu-id="a971f-128">字符串</span><span class="sxs-lookup"><span data-stu-id="a971f-128">String</span></span>|<span data-ttu-id="a971f-129">由代理计算机的服务检测到的外部 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="a971f-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="a971f-130">只读</span><span class="sxs-lookup"><span data-stu-id="a971f-130">Read-only</span></span>|
|<span data-ttu-id="a971f-131">id</span><span class="sxs-lookup"><span data-stu-id="a971f-131">id</span></span>|<span data-ttu-id="a971f-132">String</span><span class="sxs-lookup"><span data-stu-id="a971f-132">String</span></span>| <span data-ttu-id="a971f-133">OnPremisesAgent 的对象 id。</span><span class="sxs-lookup"><span data-stu-id="a971f-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="a971f-134">只读。</span><span class="sxs-lookup"><span data-stu-id="a971f-134">Read-only.</span></span>|
|<span data-ttu-id="a971f-135">machineName</span><span class="sxs-lookup"><span data-stu-id="a971f-135">machineName</span></span>|<span data-ttu-id="a971f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="a971f-136">String</span></span>|<span data-ttu-id="a971f-137">运行 aggent 的计算机的名称。</span><span class="sxs-lookup"><span data-stu-id="a971f-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="a971f-138">只读</span><span class="sxs-lookup"><span data-stu-id="a971f-138">Read-only</span></span>|
|<span data-ttu-id="a971f-139">状态</span><span class="sxs-lookup"><span data-stu-id="a971f-139">status</span></span>|<span data-ttu-id="a971f-140">string</span><span class="sxs-lookup"><span data-stu-id="a971f-140">string</span></span>| <span data-ttu-id="a971f-141">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="a971f-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="a971f-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="a971f-142">publishingType</span></span>|<span data-ttu-id="a971f-143">string</span><span class="sxs-lookup"><span data-stu-id="a971f-143">string</span></span>| <span data-ttu-id="a971f-144">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="a971f-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a971f-145">关系</span><span class="sxs-lookup"><span data-stu-id="a971f-145">Relationships</span></span>

| <span data-ttu-id="a971f-146">关系</span><span class="sxs-lookup"><span data-stu-id="a971f-146">Relationship</span></span> | <span data-ttu-id="a971f-147">类型</span><span class="sxs-lookup"><span data-stu-id="a971f-147">Type</span></span>        | <span data-ttu-id="a971f-148">说明</span><span class="sxs-lookup"><span data-stu-id="a971f-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a971f-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="a971f-149">agentGroups</span></span>|<span data-ttu-id="a971f-150">[onPremisesAgentGroup](onpremisesagentgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="a971f-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="a971f-151">向其分配**onPremisesAgent**的**onPremisesAgentGroups**的列表。</span><span class="sxs-lookup"><span data-stu-id="a971f-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="a971f-152">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a971f-152">Read-only.</span></span> <span data-ttu-id="a971f-153">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a971f-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a971f-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a971f-154">JSON representation</span></span>

<span data-ttu-id="a971f-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a971f-155">The following is a JSON representation of the resource.</span></span>

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
