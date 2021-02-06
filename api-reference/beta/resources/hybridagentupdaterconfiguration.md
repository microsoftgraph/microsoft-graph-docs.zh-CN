---
title: hybridAgentUpdaterConfiguration 资源类型
description: hybridAgentUpdaterConfiguration 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 39b378397b18337c660e76b815a80c9db398f950
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128601"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="d94a4-103">hybridAgentUpdaterConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d94a4-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="d94a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d94a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d94a4-105">租户管理员可以为每个 onPremisesPublishingProfile 配置代理可以接收更新或延迟代理更新的时间窗口。</span><span class="sxs-lookup"><span data-stu-id="d94a4-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="d94a4-106">为 onPremisesPublishingProfile 指定的 hybridAgentUpdaterConfiguration 适用于该 onPremisesPublishingProfile 内的所有代理。</span><span class="sxs-lookup"><span data-stu-id="d94a4-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="d94a4-107">例如，对于 onPremisesPublishingProfile 类型为"provisioning"的代理，步骤可能如下所示。</span><span class="sxs-lookup"><span data-stu-id="d94a4-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="d94a4-108">租户管理员可以配置为在接下来 n 天内不接收对预配代理的任何更新。</span><span class="sxs-lookup"><span data-stu-id="d94a4-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="d94a4-109">租户管理员可以配置更新窗口 (和结束) 代理可以接收更新的时间。</span><span class="sxs-lookup"><span data-stu-id="d94a4-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="d94a4-110">租户管理员可以启用 allowUpdateConfigurationOverride，这将覆盖预配代理的更新程序配置，并允许他们接收下一个可用更新。</span><span class="sxs-lookup"><span data-stu-id="d94a4-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="d94a4-111">更新程序配置中指定的 DateTime/Time 信息将转换为代理在升级期间报告的本地时区。</span><span class="sxs-lookup"><span data-stu-id="d94a4-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="d94a4-112">代理的更新将遵循以下优先级列表</span><span class="sxs-lookup"><span data-stu-id="d94a4-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="d94a4-113">如果 allowUpdateConfigurationOverride 设置为 true，将跳过租户设置的更新程序配置，当下一版本的代理可用时，代理将收到更新 (优先级为 1) 。</span><span class="sxs-lookup"><span data-stu-id="d94a4-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="d94a4-114">如果设置了延迟更新，则直到延迟更新日期时间设置为优先级 2 时 (才会更新) 。</span><span class="sxs-lookup"><span data-stu-id="d94a4-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="d94a4-115">如果设置更新窗口，则仅在该时间窗口的 24 小时内更新代理，优先级为 3 () 3。</span><span class="sxs-lookup"><span data-stu-id="d94a4-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="d94a4-116">如果租户未设置有效的更新程序配置，则代理将在下一版本的代理可用时收到更新</span><span class="sxs-lookup"><span data-stu-id="d94a4-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="d94a4-117">属性</span><span class="sxs-lookup"><span data-stu-id="d94a4-117">Properties</span></span>

| <span data-ttu-id="d94a4-118">属性</span><span class="sxs-lookup"><span data-stu-id="d94a4-118">Property</span></span>     | <span data-ttu-id="d94a4-119">类型</span><span class="sxs-lookup"><span data-stu-id="d94a4-119">Type</span></span>        | <span data-ttu-id="d94a4-120">说明</span><span class="sxs-lookup"><span data-stu-id="d94a4-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d94a4-121">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="d94a4-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="d94a4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d94a4-122">Boolean</span></span>|<span data-ttu-id="d94a4-123">指示是否跳过更新程序配置，并且代理将在下一版本的代理可用时收到更新。</span><span class="sxs-lookup"><span data-stu-id="d94a4-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="d94a4-124">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d94a4-124">deferUpdateDateTime</span></span>|<span data-ttu-id="d94a4-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d94a4-125">DateTimeOffset</span></span>|<span data-ttu-id="d94a4-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d94a4-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d94a4-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="d94a4-128">updateWindow</span></span>|[<span data-ttu-id="d94a4-129">updateWindow</span><span class="sxs-lookup"><span data-stu-id="d94a4-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="d94a4-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d94a4-130">JSON representation</span></span>

<span data-ttu-id="d94a4-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d94a4-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


