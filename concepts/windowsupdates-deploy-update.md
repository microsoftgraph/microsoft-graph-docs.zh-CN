---
title: 使用 Windows Update for Business 部署服务部署功能更新
description: 使用 Windows Update for Business 部署服务，Windows Azure AD 租户中的设备部署功能更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 92bc4c7b2b5995dd99fbb7ff549610642e4451f6
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067672"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="8e0f8-103">使用 Windows Update for Business 部署服务部署功能更新</span><span class="sxs-lookup"><span data-stu-id="8e0f8-103">Deploy a feature update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="8e0f8-104">使用 Windows Update for Business 部署服务，Windows Azure AD 租户中的设备部署更新。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="8e0f8-105">如今，部署服务[支持部署](windowsupdates-deployments.md)Windows 10更新和加速安全更新。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="8e0f8-106">本主题重点介绍功能更新的部署。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-106">This topic focuses on deployments of feature updates.</span></span> <span data-ttu-id="8e0f8-107">有关部署快速安全更新的信息，请参阅 [D部署加速安全更新](windowsupdates-deploy-expedited-update.md)。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-107">For information on deploying expedited security updates, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

<span data-ttu-id="8e0f8-108">将功能更新部署到设备时，Windows更新会向设备提供指定的更新（如果设备尚未收到更新）。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-108">When you deploy a feature update to a device, Windows Update offers the specified update to the device if it has not yet received the update.</span></span> <span data-ttu-id="8e0f8-109">例如，如果将 Windows 10 功能更新版本 20H2 部署到在功能更新管理中注册并且当前位于较旧版本的 Windows 10 的设备，则设备将更新到版本 20H2。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-109">For example, if you deploy Windows 10 feature update version 20H2 to a device that is enrolled in feature update management and is currently on an older version of Windows 10, the device updates to version 20H2.</span></span> <span data-ttu-id="8e0f8-110">如果设备已位于或高于 20H2 版本，它将保持其当前版本。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-110">If the device is already at or above version 20H2, it stays on its current version.</span></span> <span data-ttu-id="8e0f8-111">如果设备未注册功能更新管理，则此操作不会影响设备。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-111">If the device is not enrolled in feature update management, the device is not affected by this operation.</span></span>

<span data-ttu-id="8e0f8-112">只要设备仍在功能更新管理中注册，设备就不会从 Windows Update 接收任何其他功能更新，除非使用部署服务显式部署。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-112">As long as a device remains enrolled in feature update management, the device does not receive any other feature updates from Windows Update unless explicitly deployed using the deployment service.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e0f8-113">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e0f8-113">Prerequisites</span></span>

* <span data-ttu-id="8e0f8-114">设备满足 [部署服务的先决条件](windowsupdates-concept-overview.md#prerequisites)。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-114">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="8e0f8-115">在可以使用部署服务部署功能更新之前，设备必须由功能更新类别的部署服务[](windowsupdates-enroll.md)在管理中注册。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-115">Before you can use the deployment service to deploy feature updates, devices must be [enrolled in management](windowsupdates-enroll.md) by the deployment service for the feature update category.</span></span>

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a><span data-ttu-id="8e0f8-116">步骤 1： (可选) 获取可部署更新的列表</span><span class="sxs-lookup"><span data-stu-id="8e0f8-116">Step 1: (Optional) Get a list of deployable updates</span></span>

<span data-ttu-id="8e0f8-117">你可以查询部署服务目录，获取可以部署中的内容部署到设备的更新列表。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-117">You can query the deployment service catalog to get a list of updates that can be deployed to devices as content in a deployment.</span></span>

<span data-ttu-id="8e0f8-118">下面是查询部署服务可部署的所有Windows 10功能更新的示例。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-118">Below is an example of querying for all Windows 10 feature updates that are deployable by the deployment service.</span></span>

### <a name="request"></a><span data-ttu-id="8e0f8-119">请求</span><span class="sxs-lookup"><span data-stu-id="8e0f8-119">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$filter=isof('microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')
```

### <a name="response"></a><span data-ttu-id="8e0f8-120">响应</span><span class="sxs-lookup"><span data-stu-id="8e0f8-120">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "560a186a-1434-4364-8330-deb944b494ff",
            "displayName": "Windows 10, version 20H2",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "20H2"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "5e436dae-56bd-4925-bf8b-acf550e07227",
            "displayName": "Windows 10, version 2004",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "2004"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="8e0f8-121">步骤 2：创建部署</span><span class="sxs-lookup"><span data-stu-id="8e0f8-121">Step 2: Create a deployment</span></span>

<span data-ttu-id="8e0f8-122">[部署](/graph/api/resources/windowsupdates-deployment)指定要部署的内容、如何以及何时部署内容以及目标设备。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-122">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="8e0f8-123">创建部署后，将自动将部署访问群体创建为关系。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-123">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="8e0f8-124">下面是使用配置部署计划及监视规则的可选设置创建功能[更新部署](windowsupdates-schedule-deployment.md)[的示例](windowsupdates-manage-monitoring-rules.md)。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-124">Below is an example of creating a deployment of a feature update, with optional settings configuring the [deployment schedule](windowsupdates-schedule-deployment.md) and [monitoring rules](windowsupdates-manage-monitoring-rules.md).</span></span> <span data-ttu-id="8e0f8-125">目标设备在下一步中指定。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-125">The targeted devices are specified in the next step.</span></span>

> [!NOTE]
> <span data-ttu-id="8e0f8-126">如果在创建 [部署时未指定](/graph/api/resources/windowsupdates-monitoringrule) 监视规则，则创建默认监视规则。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-126">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a deployment, a default monitoring rule is created.</span></span> <span data-ttu-id="8e0f8-127">此默认监视规则具有 **信号**、阈值 和 `rollback`  `20` **操作** `alertError` 。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-127">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="8e0f8-128">在 API 的未来更新中，此行为将更改，并且不会创建默认监视规则。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-128">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

### <a name="request"></a><span data-ttu-id="8e0f8-129">请求</span><span class="sxs-lookup"><span data-stu-id="8e0f8-129">Request</span></span>

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
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        },
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

### <a name="response"></a><span data-ttu-id="8e0f8-130">响应</span><span class="sxs-lookup"><span data-stu-id="8e0f8-130">Response</span></span>

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
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "startDateTime": null,
            "endDateTime": null
        },
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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="8e0f8-131">步骤 3：将设备分配给部署访问群体</span><span class="sxs-lookup"><span data-stu-id="8e0f8-131">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="8e0f8-132">创建部署后，你可以将设备分配给部署 [访问群体](/graph/api/resources/windowsupdates-deploymentaudience)。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-132">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="8e0f8-133">设备可以直接分配，或通过可 [更新的资产组进行分配](/graph/api/resources/windowsupdates-updatableassetgroup)。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-133">Devices can be assigned directly, or via [updatable asset groups](/graph/api/resources/windowsupdates-updatableassetgroup).</span></span> <span data-ttu-id="8e0f8-134">成功更新部署访问群体后，Windows更新开始根据部署设置向相关设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-134">Once the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="8e0f8-135">当设备添加到部署访问群体的成员或排除集合时 (将自动注册服务，即 [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) 对象在部署访问群体中) 。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-135">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (i.e. an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="8e0f8-136">下面是添加可更新资源组和 Azure AD 设备作为部署受众成员的示例，同时还排除特定的 Azure AD 设备。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-136">Below is an example of adding updatable asset groups and Azure AD devices as members of the deployment audience, while also excluding a specific Azure AD device.</span></span>

### <a name="request"></a><span data-ttu-id="8e0f8-137">请求</span><span class="sxs-lookup"><span data-stu-id="8e0f8-137">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        }
    ],
    "addExclusions": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="8e0f8-138">响应</span><span class="sxs-lookup"><span data-stu-id="8e0f8-138">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="8e0f8-139">部署期间</span><span class="sxs-lookup"><span data-stu-id="8e0f8-139">During a deployment</span></span>

<span data-ttu-id="8e0f8-140">在部署过程中，可以通过更新部署的状态来暂停部署，也可以更新其访问群体成员和排除项。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-140">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="8e0f8-141">部署后</span><span class="sxs-lookup"><span data-stu-id="8e0f8-141">After a deployment</span></span>

<span data-ttu-id="8e0f8-142">在最初向部署访问群体分配的所有设备都提供更新后，由于设备连接等因素，并非所有设备都启动或完成了更新。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-142">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="8e0f8-143">只要部署仍然存在，Windows只要重新连接，更新就会继续为分配的设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="8e0f8-143">As long as the deployment still exists, Windows Update continues to offer the update to the assigned devices whenever they reconnect.</span></span>

