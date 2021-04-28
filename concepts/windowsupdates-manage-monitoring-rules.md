---
title: 使用 Windows Update for Business 部署服务管理部署的监视规则
description: 对于部署服务启动的部署，可以使用监视规则根据部署信号配置警报和自动操作。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 7468bef695b704ef40b630e3f0e332e97fb12031
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067670"
---
# <a name="manage-monitoring-rules-for-a-feature-update-deployment-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="1d5bb-103">使用 Windows Update for Business 部署服务管理功能更新部署的监视规则</span><span class="sxs-lookup"><span data-stu-id="1d5bb-103">Manage monitoring rules for a feature update deployment using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="1d5bb-104">对于部署服务启动的部署，可以使用监视规则根据部署信号配置警报和自动操作。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-104">For deployments initiated by the deployment service, you can use a monitoring rule to configure alerts and automated actions based on deployment signals.</span></span>

<span data-ttu-id="1d5bb-105">监视规则与部署功能Windows 10兼容。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-105">Monitoring rules are compatible with deployments of Windows 10 feature updates.</span></span>

> [!NOTE]
> <span data-ttu-id="1d5bb-106">如果在创建[部署时未指定](/graph/api/resources/windowsupdates-monitoringrule)监视规则，将创建默认[](/graph/api/resources/windowsupdates-deployment)监视规则。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-106">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a [deployment](/graph/api/resources/windowsupdates-deployment), a default monitoring rule is created.</span></span> <span data-ttu-id="1d5bb-107">此默认监视规则具有 **信号**、阈值 和 `rollback`  `20` **操作** `alertError` 。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-107">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="1d5bb-108">在 API 的未来更新中，此行为将更改，并且不会创建默认监视规则。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-108">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

## <a name="step-1-create-a-monitoring-rule"></a><span data-ttu-id="1d5bb-109">步骤 1：创建监视规则</span><span class="sxs-lookup"><span data-stu-id="1d5bb-109">Step 1: Create a monitoring rule</span></span>

<span data-ttu-id="1d5bb-110">您可以通过配置 [监视](/graph/api/resources/windowsupdates-monitoringrule) 设置为部署创建 [监视规则](/graph/api/resources/windowsupdates-monitoringsettings)。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-110">You can create a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) for a deployment by configuring the [monitoring settings](/graph/api/resources/windowsupdates-monitoringsettings).</span></span> <span data-ttu-id="1d5bb-111">每个 [部署](/graph/api/resources/windowsupdates-deployments) 一次可以有一个活动的监视规则。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-111">Each [deployment](/graph/api/resources/windowsupdates-deployments) can have one active monitoring rule at a time.</span></span>

<span data-ttu-id="1d5bb-112">监视规则由三个部分组成：</span><span class="sxs-lookup"><span data-stu-id="1d5bb-112">Monitoring rules consist of three components:</span></span>
* <span data-ttu-id="1d5bb-113">**signal**：部署服务要监视的更新问题的类型。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-113">**signal**: The type of update issue to be monitored by the deployment service.</span></span>
* <span data-ttu-id="1d5bb-114">**threshold：** 当此百分比的设备发出指定信号时，将触发监视规则。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-114">**threshold**: When this percentage of devices emit the specified signal, the monitoring rule is triggered.</span></span>
* <span data-ttu-id="1d5bb-115">**action：** 触发监视规则时要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-115">**action**: The action to take when the monitoring rule is triggered.</span></span>

<span data-ttu-id="1d5bb-116">下面是在创建部署的同时为部署创建监视规则的示例。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-116">Below is an example of creating a monitoring rule for a deployment at the same time as creating the deployment.</span></span>

### <a name="request"></a><span data-ttu-id="1d5bb-117">请求</span><span class="sxs-lookup"><span data-stu-id="1d5bb-117">Request</span></span>

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
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

### <a name="response"></a><span data-ttu-id="1d5bb-118">响应</span><span class="sxs-lookup"><span data-stu-id="1d5bb-118">Response</span></span>

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
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-unpause-a-deployment-that-was-paused-by-a-monitoring-rule"></a><span data-ttu-id="1d5bb-119">步骤 2：取消使用由监视规则暂停的部署</span><span class="sxs-lookup"><span data-stu-id="1d5bb-119">Step 2: Unpause a deployment that was paused by a monitoring rule</span></span>
<span data-ttu-id="1d5bb-120">当监视规则触发时，它将有机会调查可能导致应用更新的更新问题。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-120">When a monitoring rule triggers, it provides the opportunity to investigate update issues that may have lead to it being applied.</span></span> <span data-ttu-id="1d5bb-121">调查后，你可能希望恢复部署。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-121">After investigation, you may wish to resume the deployment.</span></span> <span data-ttu-id="1d5bb-122">有两种方法可以这样做：删除监视规则或更新监视规则阈值。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-122">There are two ways to do so: removing the monitoring rule or updating the monitoring rule threshold.</span></span>

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a><span data-ttu-id="1d5bb-123">示例：通过删除监视规则恢复部署</span><span class="sxs-lookup"><span data-stu-id="1d5bb-123">Example: Resume deployment by removing a monitoring rule</span></span>
<span data-ttu-id="1d5bb-124">触发暂停部署的监视规则时，恢复部署的一种方式是删除该规则。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-124">When a monitoring rule that pauses the deployment is triggered, one way to resume the deployment is to remove the rule.</span></span>

<span data-ttu-id="1d5bb-125">下面是通过删除规则恢复部署的示例。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-125">Below is an example of resuming the deployment by removing the rule.</span></span>

#### <a name="request"></a><span data-ttu-id="1d5bb-126">请求</span><span class="sxs-lookup"><span data-stu-id="1d5bb-126">Request</span></span>

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": []
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="1d5bb-127">响应</span><span class="sxs-lookup"><span data-stu-id="1d5bb-127">Response</span></span>

``` http
HTTP/1.1 202 Accepted
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
        "monitoring": {
            "monitoringRules": []
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a><span data-ttu-id="1d5bb-128">示例：通过更新监视规则阈值恢复部署</span><span class="sxs-lookup"><span data-stu-id="1d5bb-128">Example: Resume deployment by updating a monitoring rule threshold</span></span>
<span data-ttu-id="1d5bb-129">恢复部署的另一种方式是更改相关监视规则的阈值。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-129">Another way to resume the deployment is to change the threshold of the relevant monitoring rule.</span></span> <span data-ttu-id="1d5bb-130">当达到新阈值时，操作 (，) `pauseDeployment` 将再次触发。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-130">When the new threshold is reached, the action (in this case, `pauseDeployment`) will be triggered again.</span></span> 

<span data-ttu-id="1d5bb-131">下面是通过更改监视规则阈值恢复部署的示例。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-131">Below is an example of resuming the deployment by changing the monitoring rule threshold.</span></span> <span data-ttu-id="1d5bb-132">此示例还说明如何编辑任何现有的监视规则（即使尚未达到其阈值）以及如何在没有监控规则的部署上创建监视规则。</span><span class="sxs-lookup"><span data-stu-id="1d5bb-132">This example also illustrates how to edit any existing monitoring rule, even if its threshold has not yet been met, as well as how to create a monitoring rule on a deployment that does not have one.</span></span>

#### <a name="request"></a><span data-ttu-id="1d5bb-133">请求</span><span class="sxs-lookup"><span data-stu-id="1d5bb-133">Request</span></span>

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="1d5bb-134">响应</span><span class="sxs-lookup"><span data-stu-id="1d5bb-134">Response</span></span>

``` http
HTTP/1.1 202 Accepted
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
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```