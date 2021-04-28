---
title: 使用 Windows Update for Business 部署服务安排部署
description: 使用部署服务部署更新时，可以计划部署，以便设备在未来日期接收更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 461b40ef1e25d6a1943c70456404e7a48bf73d8c
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067669"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="6a481-103">使用 Windows Update for Business 部署服务安排部署</span><span class="sxs-lookup"><span data-stu-id="6a481-103">Schedule a deployment using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="6a481-104">使用部署服务部署更新时，可以计划部署，以便设备在未来日期接收更新。</span><span class="sxs-lookup"><span data-stu-id="6a481-104">When deploying an update using the deployment service, you can schedule the deployment so that devices receive the update at a future date.</span></span>

<span data-ttu-id="6a481-105">计划功能与部署[功能Windows 10](windowsupdates-deployments.md)兼容。</span><span class="sxs-lookup"><span data-stu-id="6a481-105">Scheduling features are compatible with [deployments](windowsupdates-deployments.md) of Windows 10 feature updates.</span></span>

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a><span data-ttu-id="6a481-106">计划部署在未来日期开始</span><span class="sxs-lookup"><span data-stu-id="6a481-106">Schedule a deployment to start at a future date</span></span>

<span data-ttu-id="6a481-107">可以通过配置部署设置，计划部署在未来日期 [开始](/graph/api/resources/windowsupdates-rolloutsettings)。</span><span class="sxs-lookup"><span data-stu-id="6a481-107">You can schedule a deployment to start at a future date by configuring its [rollout settings](/graph/api/resources/windowsupdates-rolloutsettings).</span></span> <span data-ttu-id="6a481-108">在下面的示例中，分配了部署的所有设备都将在 2021 年 7 月 1 日获得更新。</span><span class="sxs-lookup"><span data-stu-id="6a481-108">In the example below, all devices assigned the deployment will be offered the update on July 1, 2021.</span></span>

### <a name="request"></a><span data-ttu-id="6a481-109">请求</span><span class="sxs-lookup"><span data-stu-id="6a481-109">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
        }
    }
}
```

### <a name="response"></a><span data-ttu-id="6a481-110">响应</span><span class="sxs-lookup"><span data-stu-id="6a481-110">Response</span></span>

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": null,
            "durationBetweenOffers": "P1D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a><span data-ttu-id="6a481-111">在一段时间内部署阶段</span><span class="sxs-lookup"><span data-stu-id="6a481-111">Stage a deployment over a period of time</span></span>

<span data-ttu-id="6a481-112">还可以计划部署，以便向分配的设备提供逐步推出中的更新，该部署会逐步进行。</span><span class="sxs-lookup"><span data-stu-id="6a481-112">You can also schedule a deployment so that assigned devices are offered the update in a gradual rollout that is staged over time.</span></span> <span data-ttu-id="6a481-113">更新按固定间隔提供给分配到部署的设备的子集，推出的总持续时间由结束日期或产品/服务费率决定。</span><span class="sxs-lookup"><span data-stu-id="6a481-113">The update is offered to subsets of devices assigned to the deployment at regular intervals, with the total duration of the rollout determined by either an end date or offering rate.</span></span> <span data-ttu-id="6a481-114">你可以将逐步推出视为类似于定期日历事件系列。</span><span class="sxs-lookup"><span data-stu-id="6a481-114">You can think of a gradual rollout as similar to a recurring calendar event series.</span></span>

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a><span data-ttu-id="6a481-115">示例：在开始日期和结束日期之间定期部署</span><span class="sxs-lookup"><span data-stu-id="6a481-115">Example: Stage a deployment at regular intervals between start and end dates</span></span>

<span data-ttu-id="6a481-116">在一定时间阶段部署一种方式是设置部署的 **endDateTime。**</span><span class="sxs-lookup"><span data-stu-id="6a481-116">One way to stage a deployment over time is to set the **endDateTime** of the deployment.</span></span> <span data-ttu-id="6a481-117">分配给部署的所有设备都将在 **startDateTime** 和 **endDateTime** 之间的窗口中提供更新。</span><span class="sxs-lookup"><span data-stu-id="6a481-117">All devices assigned to the deployment will be offered the update within the window between the **startDateTime** and **endDateTime**.</span></span> <span data-ttu-id="6a481-118">如果 **未指定 startDateTime，** 则分配设备后将立即开始部署。</span><span class="sxs-lookup"><span data-stu-id="6a481-118">If the **startDateTime** is not specified, then the deployment will begin as soon as devices are assigned.</span></span>


<span data-ttu-id="6a481-119">本示例中，配置了一个新部署，以便从 2021 年 7 月 1 日开始，每周向一组新设备提供更新 (**durationBetweenOffers** 设置为) 七天。</span><span class="sxs-lookup"><span data-stu-id="6a481-119">In this example, you configure a new deployment so that a new set of devices is offered the update every week (**durationBetweenOffers** set to seven days), starting on July 1, 2021.</span></span> <span data-ttu-id="6a481-120">在 2021 年 8 月 1 日之前，会向所有设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="6a481-120">All devices are offered the update before August 1, 2021.</span></span>

#### <a name="request"></a><span data-ttu-id="6a481-121">请求</span><span class="sxs-lookup"><span data-stu-id="6a481-121">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="6a481-122">响应</span><span class="sxs-lookup"><span data-stu-id="6a481-122">Response</span></span>

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "rollout": {
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a><span data-ttu-id="6a481-123">示例：定期部署，每个产品/服务具有指定数量的设备</span><span class="sxs-lookup"><span data-stu-id="6a481-123">Example: Stage a deployment at regular intervals with a specified number of devices at each offer</span></span>

<span data-ttu-id="6a481-124">在一段时间后部署阶段的另一种方式是使用 配置产品/服务费率 `devicesPerOffer` 。</span><span class="sxs-lookup"><span data-stu-id="6a481-124">Another way to stage a deployment over time is to configure the offering rate using `devicesPerOffer`.</span></span> <span data-ttu-id="6a481-125">分配给部署的设备将按照指定的速率提供更新，直到所有设备都获得更新。</span><span class="sxs-lookup"><span data-stu-id="6a481-125">Devices assigned to the deployment will be offered the update according to the specified rate until all devices have been offered the update.</span></span>

<span data-ttu-id="6a481-126">本示例中，配置了一个新部署，以便从 2021 年 7 月 1 日开始，每周向一组新设备提供更新 (**durationBetweenOffers** 设置为) 七天。</span><span class="sxs-lookup"><span data-stu-id="6a481-126">In this example, you configure a new deployment so that a new set of devices is offered the update every week (**durationBetweenOffers** set to seven days), starting on July 1, 2021.</span></span> <span data-ttu-id="6a481-127">一次向 100 台设备提供更新，直到所有设备都获得更新。</span><span class="sxs-lookup"><span data-stu-id="6a481-127">100 devices are offered the update at a time until all devices have been offered the update.</span></span>

#### <a name="request"></a><span data-ttu-id="6a481-128">请求</span><span class="sxs-lookup"><span data-stu-id="6a481-128">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "rollout": {
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="6a481-129">响应</span><span class="sxs-lookup"><span data-stu-id="6a481-129">Response</span></span>

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "rollout": {
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "endDateTime": null
        },
        "monitoring": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```