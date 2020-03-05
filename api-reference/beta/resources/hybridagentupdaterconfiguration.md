---
title: hybridAgentUpdaterConfiguration 资源类型
description: hybridAgentUpdaterConfiguration 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c10173d099ac7c2ad9714b0240f306e783fdd6da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496808"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="0d724-103">hybridAgentUpdaterConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d724-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="0d724-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0d724-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d724-105">租户管理员可以为每个 onPremisesPublishingProfile 配置一个时间段，在此时段内，代理可以接收更新或将更新推迟到代理。</span><span class="sxs-lookup"><span data-stu-id="0d724-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="0d724-106">为 onPremisesPublishingProfile 指定的 hybridAgentUpdaterConfiguration 适用于该 onPremisesPublishingProfile 中的所有代理。</span><span class="sxs-lookup"><span data-stu-id="0d724-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="0d724-107">例如，对于 onPremisesPublishingProfile 中类型为 "预配" 的代理，这些步骤可能如下所示。</span><span class="sxs-lookup"><span data-stu-id="0d724-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="0d724-108">租户管理员可以配置为在接下来的 n 天中不接收对预配代理的任何更新。</span><span class="sxs-lookup"><span data-stu-id="0d724-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="0d724-109">租户管理员可以配置更新窗口（开始和结束时间），在此期间，代理可以 recive 更新。</span><span class="sxs-lookup"><span data-stu-id="0d724-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="0d724-110">租户管理员可以启用 allowUpdateConfigurationOverride，这将覆盖预配代理的更新 configutration，并 alows 他们接收下一个可用的更新。</span><span class="sxs-lookup"><span data-stu-id="0d724-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="0d724-111">在更新配置过程中指定的 DateTime/Time 信息将转换为 evaluvation 期间代理报告的本地时区。</span><span class="sxs-lookup"><span data-stu-id="0d724-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="0d724-112">代理的更新将遵循以下优先级列表</span><span class="sxs-lookup"><span data-stu-id="0d724-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="0d724-113">如果将 allowUpdateConfigurationOverride 设置为 true，则将跳过租户设置的更新配置，并且代理将在下一版本的代理可用时收到更新（优先级为1）。</span><span class="sxs-lookup"><span data-stu-id="0d724-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="0d724-114">如果设置了延迟更新，将不会更新代理，直到延迟更新日期时间（优先级2）。</span><span class="sxs-lookup"><span data-stu-id="0d724-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="0d724-115">如果设置了 "更新" 窗口，则代理将仅在24小时内（优先级为3）的该时间段内更新。</span><span class="sxs-lookup"><span data-stu-id="0d724-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="0d724-116">如果租户未设置有效的更新程序配置，则代理将在下一版本的代理可用时收到更新。</span><span class="sxs-lookup"><span data-stu-id="0d724-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="0d724-117">属性</span><span class="sxs-lookup"><span data-stu-id="0d724-117">Properties</span></span>

| <span data-ttu-id="0d724-118">属性</span><span class="sxs-lookup"><span data-stu-id="0d724-118">Property</span></span>     | <span data-ttu-id="0d724-119">类型</span><span class="sxs-lookup"><span data-stu-id="0d724-119">Type</span></span>        | <span data-ttu-id="0d724-120">说明</span><span class="sxs-lookup"><span data-stu-id="0d724-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d724-121">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="0d724-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="0d724-122">布尔</span><span class="sxs-lookup"><span data-stu-id="0d724-122">Boolean</span></span>|<span data-ttu-id="0d724-123">指示是否将跳过更新配置，并且代理将在下一版本的代理可用时收到更新。</span><span class="sxs-lookup"><span data-stu-id="0d724-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="0d724-124">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0d724-124">deferUpdateDateTime</span></span>|<span data-ttu-id="0d724-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d724-125">DateTimeOffset</span></span>|<span data-ttu-id="0d724-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d724-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d724-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="0d724-128">updateWindow</span></span>|[<span data-ttu-id="0d724-129">updateWindow</span><span class="sxs-lookup"><span data-stu-id="0d724-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="0d724-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d724-130">JSON representation</span></span>

<span data-ttu-id="0d724-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d724-131">The following is a JSON representation of the resource.</span></span>

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
