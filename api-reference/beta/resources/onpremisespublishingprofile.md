---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 8e74374baa397c292d323dc0520833a7318cbe79
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134895"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="2ca3a-103">onPremisesPublishingProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ca3a-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="2ca3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ca3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ca3a-105">各种 Azure (例如，Azure Active Directory Connect [Passthrough](/azure/active-directory/hybrid/how-to-connect-pta)Authentication、Workday [to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial)和应用程序 [代理](https://aka.ms/whyappproxy) 允许从企业网络外部访问各种本地资源。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="2ca3a-106">[可以将由](onpremisesagent.md) (安装的应用程序代理或) 连接器[](connector.md)本地代理配置为将请求路由到特定的[已发布资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="2ca3a-107">[通过应用程序](onpremisesagentgroup.md) (代理的代理组[](connectorgroup.md)或) 组，管理员可以分配特定代理，为发布的特定本地资源提供服务。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="2ca3a-108">管理员还可以将多个代理分组在一起，然后将每个已发布的资源分配给代理组。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="2ca3a-109">同一本地发布类型的整个实体集由 **onPremisesPublishingProfile 表示**。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="2ca3a-110">方法</span><span class="sxs-lookup"><span data-stu-id="2ca3a-110">Methods</span></span>

| <span data-ttu-id="2ca3a-111">方法</span><span class="sxs-lookup"><span data-stu-id="2ca3a-111">Method</span></span>       | <span data-ttu-id="2ca3a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ca3a-112">Return Type</span></span> | <span data-ttu-id="2ca3a-113">说明</span><span class="sxs-lookup"><span data-stu-id="2ca3a-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2ca3a-114">获取 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="2ca3a-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="2ca3a-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="2ca3a-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="2ca3a-116">读取 **onPremisesPublishingProfile** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="2ca3a-117">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="2ca3a-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="2ca3a-118">无</span><span class="sxs-lookup"><span data-stu-id="2ca3a-118">None</span></span> | <span data-ttu-id="2ca3a-119">更新 [onPremisesPublishingProfile](onpremisespublishingprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ca3a-120">属性</span><span class="sxs-lookup"><span data-stu-id="2ca3a-120">Properties</span></span>

| <span data-ttu-id="2ca3a-121">属性</span><span class="sxs-lookup"><span data-stu-id="2ca3a-121">Property</span></span>     | <span data-ttu-id="2ca3a-122">类型</span><span class="sxs-lookup"><span data-stu-id="2ca3a-122">Type</span></span>        | <span data-ttu-id="2ca3a-123">说明</span><span class="sxs-lookup"><span data-stu-id="2ca3a-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ca3a-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ca3a-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="2ca3a-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ca3a-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="2ca3a-126">代表 **hybridAgentUpdaterConfiguration** 对象。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="2ca3a-127">id</span><span class="sxs-lookup"><span data-stu-id="2ca3a-127">id</span></span>|<span data-ttu-id="2ca3a-128">字符串</span><span class="sxs-lookup"><span data-stu-id="2ca3a-128">String</span></span>| <span data-ttu-id="2ca3a-129">表示发布类型。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-129">Represents a publishing type.</span></span> <span data-ttu-id="2ca3a-130">可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="2ca3a-131">只读。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-131">Read-only.</span></span>|
|<span data-ttu-id="2ca3a-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2ca3a-132">isEnabled</span></span>|<span data-ttu-id="2ca3a-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca3a-133">Boolean</span></span>| <span data-ttu-id="2ca3a-134">表示是否 [为租户启用了 Azure AD](https://aka.ms/whyappproxy) 应用程序代理。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2ca3a-135">关系</span><span class="sxs-lookup"><span data-stu-id="2ca3a-135">Relationships</span></span>

| <span data-ttu-id="2ca3a-136">关系</span><span class="sxs-lookup"><span data-stu-id="2ca3a-136">Relationship</span></span> | <span data-ttu-id="2ca3a-137">类型</span><span class="sxs-lookup"><span data-stu-id="2ca3a-137">Type</span></span>        | <span data-ttu-id="2ca3a-138">说明</span><span class="sxs-lookup"><span data-stu-id="2ca3a-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ca3a-139">agentGroups</span><span class="sxs-lookup"><span data-stu-id="2ca3a-139">agentGroups</span></span>|<span data-ttu-id="2ca3a-140">[onPremisesAgentGroup](onpremisesagentgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ca3a-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="2ca3a-141">现有 **onPremisesAgentGroup 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="2ca3a-142">只读。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-142">Read-only.</span></span> <span data-ttu-id="2ca3a-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-143">Nullable.</span></span>|
|<span data-ttu-id="2ca3a-144">agents</span><span class="sxs-lookup"><span data-stu-id="2ca3a-144">agents</span></span>|<span data-ttu-id="2ca3a-145">[onPremisesAgent](onpremisesagent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ca3a-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="2ca3a-146">现有 **onPremisesAgent 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="2ca3a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-147">Read-only.</span></span> <span data-ttu-id="2ca3a-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-148">Nullable.</span></span>|
|<span data-ttu-id="2ca3a-149">connectorGroups</span><span class="sxs-lookup"><span data-stu-id="2ca3a-149">connectorGroups</span></span>|<span data-ttu-id="2ca3a-150">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ca3a-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="2ca3a-151">通过应用程序代理发布的应用程序的现有 **connectorGroup** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="2ca3a-152">只读。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-152">Read-only.</span></span> <span data-ttu-id="2ca3a-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-153">Nullable.</span></span>|
|<span data-ttu-id="2ca3a-154">连接器</span><span class="sxs-lookup"><span data-stu-id="2ca3a-154">connectors</span></span>|<span data-ttu-id="2ca3a-155">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ca3a-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="2ca3a-156">通过应用程序 **代理** 发布的应用程序的现有连接器对象列表。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="2ca3a-157">只读。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-157">Read-only.</span></span> <span data-ttu-id="2ca3a-158">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-158">Nullable.</span></span>|
|<span data-ttu-id="2ca3a-159">publishedResources</span><span class="sxs-lookup"><span data-stu-id="2ca3a-159">publishedResources</span></span>|<span data-ttu-id="2ca3a-160">[publishedResource](publishedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ca3a-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="2ca3a-161">现有 **publishedResource 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="2ca3a-162">只读。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-162">Read-only.</span></span> <span data-ttu-id="2ca3a-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ca3a-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ca3a-164">JSON representation</span></span>

<span data-ttu-id="2ca3a-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ca3a-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



