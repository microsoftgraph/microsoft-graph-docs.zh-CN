---
title: 使用 Windows Update for Business 部署服务部署快速安全更新
description: 借助 Windows Update for Business 部署服务，你可以将加速 Windows 安全更新部署到 Azure AD 租户中的设备，以防出现紧急情况，并需要立即部署安全更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: d64cb09545d1ce664b017ba3fcbcd5989d0f2a25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210190"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="93fa1-103">使用 Windows Update for Business 部署服务部署快速安全更新</span><span class="sxs-lookup"><span data-stu-id="93fa1-103">Deploy an expedited security update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="93fa1-104">使用 Windows Update for Business 部署服务，Windows Azure AD 租户中的设备部署更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="93fa1-105">如今，部署服务[支持部署](windowsupdates-deployments.md)Windows 10更新和加速安全更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="93fa1-106">本主题重点介绍快速安全更新的部署。</span><span class="sxs-lookup"><span data-stu-id="93fa1-106">This topic focuses on deployments of expedited security updates.</span></span> <span data-ttu-id="93fa1-107">有关部署功能更新的信息，请参阅 [部署功能更新](windowsupdates-deploy-update.md)。</span><span class="sxs-lookup"><span data-stu-id="93fa1-107">For information on deploying feature updates, see [Deploy a feature update](windowsupdates-deploy-update.md).</span></span>

<span data-ttu-id="93fa1-108">安装安全更新会覆盖Windows更新的延迟策略，以便尽快安装更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-108">Expediting a security update overrides Windows Update for Business deferral policies so that the update is installed as quickly as possible.</span></span> <span data-ttu-id="93fa1-109">当出现关键安全事件并且需要比正常情况更快速地部署最新更新时，它非常有用。</span><span class="sxs-lookup"><span data-stu-id="93fa1-109">It can be useful when critical security events arise and you need to deploy the latest updates more rapidly than normal.</span></span> <span data-ttu-id="93fa1-110">但是，虽然它可以帮助实现针对特定安全更新的合规性目标，但它并非旨在每月使用一次。</span><span class="sxs-lookup"><span data-stu-id="93fa1-110">However, while it can help to achieve compliance targets against a specific security update, it is not designed to be used every month.</span></span> <span data-ttu-id="93fa1-111">相反，请考虑使用 [更新的合规性截止时间](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines)。</span><span class="sxs-lookup"><span data-stu-id="93fa1-111">Instead, consider using [compliance deadlines for updates](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines).</span></span>

<span data-ttu-id="93fa1-112">将加速安全更新部署到设备时，Windows更新会向设备提供最新的适用更新（如果设备尚未收到具有指定发布日期的更新）。</span><span class="sxs-lookup"><span data-stu-id="93fa1-112">When you deploy an expedited security update to a device, Windows Update offers the latest applicable update to the device if it has not yet received the update with the specified release date.</span></span> <span data-ttu-id="93fa1-113">例如，如果将 2021 Windows 10 2021 年 4 月 13 日发布的更新安全更新部署到当前没有更新的设备，则设备将收到快速更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-113">For example, if you deploy the Windows 10 security update released on April 13, 2021 to a device that does not currently have the update, the device receives an expedited update.</span></span> <span data-ttu-id="93fa1-114">如果设备已具有指定的更新或更新版本，则它不会收到加速更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-114">If the device already has the specified update or newer, it does not receive an expedited update.</span></span>

<span data-ttu-id="93fa1-115">加速安全更新还具有以下特征：</span><span class="sxs-lookup"><span data-stu-id="93fa1-115">Expedited security updates also have the following characteristics:</span></span>

* <span data-ttu-id="93fa1-116">更新立即启动，而不是等待下一次定期更新扫描，默认情况下每 22 小时进行一次。</span><span class="sxs-lookup"><span data-stu-id="93fa1-116">The update starts right away rather than waiting for the next regular update scan, which occurs once every 22 hours by default.</span></span>
* <span data-ttu-id="93fa1-117">更新将尽快下载和安装。</span><span class="sxs-lookup"><span data-stu-id="93fa1-117">The update downloads and installs as quickly as possible.</span></span>
* <span data-ttu-id="93fa1-118">更新过程会覆盖配置的设备策略设置，例如，在设备被强制重启之前几天。</span><span class="sxs-lookup"><span data-stu-id="93fa1-118">The update process overrides configured device policy settings, such as days until the device is forced to restart.</span></span> <span data-ttu-id="93fa1-119">安装快速更新后，设备将返回到当前策略设置。</span><span class="sxs-lookup"><span data-stu-id="93fa1-119">After the expedited update is installed, the device returns to the current policy settings.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93fa1-120">先决条件</span><span class="sxs-lookup"><span data-stu-id="93fa1-120">Prerequisites</span></span>

* <span data-ttu-id="93fa1-121">设备满足 [部署服务的先决条件](windowsupdates-concept-overview.md#prerequisites)。</span><span class="sxs-lookup"><span data-stu-id="93fa1-121">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="93fa1-122">设备已安装[KB4023057 - Windows 10 Update Service](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a)组件更新 (更新) 。</span><span class="sxs-lookup"><span data-stu-id="93fa1-122">Devices have installed the update described in [KB4023057 - Update for Windows 10 Update Service components](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) (or newer).</span></span>

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a><span data-ttu-id="93fa1-123">步骤 1： (可选) 获取可安装更新的列表</span><span class="sxs-lookup"><span data-stu-id="93fa1-123">Step 1: (Optional) Get a list of expeditable updates</span></span>

<span data-ttu-id="93fa1-124">你可以查询部署服务目录，获取更新列表，这些更新可以加速到设备作为部署中的内容。</span><span class="sxs-lookup"><span data-stu-id="93fa1-124">You can query the deployment service catalog to get a list of updates that can be expedited to devices as content in a deployment.</span></span>

<span data-ttu-id="93fa1-125">安全更新由 [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) 类型表示 **，qualityUpdateClassification** 为 `security` 。</span><span class="sxs-lookup"><span data-stu-id="93fa1-125">Security updates are represented by the [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) type, with a **qualityUpdateClassification** of `security`.</span></span> <span data-ttu-id="93fa1-126">所有Windows 10分类为安全更新的更新质量更新都可以加速，并且使用设置为 的 **isExpeditable** 属性进行 `true` 标记以标识它们。</span><span class="sxs-lookup"><span data-stu-id="93fa1-126">All Windows 10 quality updates that are classified as security updates can be expedited and are tagged with the **isExpeditable** property set to `true` to identify them.</span></span>

<span data-ttu-id="93fa1-127">下面是一个查询所有 Windows 10 安全更新的示例，这些安全更新可通过部署服务作为快速更新进行部署。</span><span class="sxs-lookup"><span data-stu-id="93fa1-127">Below is an example of querying for all Windows 10 security updates that can be deployed as expedited updates by the deployment service.</span></span> <span data-ttu-id="93fa1-128">Microsoft 建议只显示三个最新更新，因此该示例包括 `$top=3` 。</span><span class="sxs-lookup"><span data-stu-id="93fa1-128">Microsoft recommends to only show the three most current updates, so the example includes `$top=3`.</span></span>

### <a name="request"></a><span data-ttu-id="93fa1-129">请求</span><span class="sxs-lookup"><span data-stu-id="93fa1-129">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a><span data-ttu-id="93fa1-130">响应</span><span class="sxs-lookup"><span data-stu-id="93fa1-130">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "bd9554dc-2737-4e3c-b794-fa2b8b3f4a30",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "68860630-c2d0-4dd2-8c4b-9b9737ee5081",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "aa336b13-db33-4d94-89ea-90e43e4ad30b",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="93fa1-131">步骤 2：创建部署</span><span class="sxs-lookup"><span data-stu-id="93fa1-131">Step 2: Create a deployment</span></span>

<span data-ttu-id="93fa1-132">[部署](/graph/api/resources/windowsupdates-deployment)指定要部署的内容、如何以及何时部署内容以及目标设备。</span><span class="sxs-lookup"><span data-stu-id="93fa1-132">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="93fa1-133">对于质量更新，使用目标合规性日期指定内容。</span><span class="sxs-lookup"><span data-stu-id="93fa1-133">For quality updates, the content is specified using a target compliance date.</span></span> <span data-ttu-id="93fa1-134">创建部署后，将自动将部署访问群体创建为关系。</span><span class="sxs-lookup"><span data-stu-id="93fa1-134">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="93fa1-135">将加速安全更新部署到设备时，Windows更新会提供一个更新，将设备超过指定的最低合规性级别。</span><span class="sxs-lookup"><span data-stu-id="93fa1-135">When you deploy an expedited security update to a device, Windows Update offers an update that brings the device above the minimum compliance level specified.</span></span> <span data-ttu-id="93fa1-136">根据每个设备扫描和更新时间，某些设备可能会收到更新 (例如，如果有比所需最低合规性级别) 更新更新的更新，但所有设备都符合指定的安全更新合规性标准。</span><span class="sxs-lookup"><span data-stu-id="93fa1-136">Depending on when each device scans and updates, some devices may receive newer updates (e.g. if there is a newer security update than the one corresponding to the desired minimum compliance level), but all devices meet the specified security update compliance standard.</span></span> <span data-ttu-id="93fa1-137">这种提供最新适用更新的行为（由设置为默认值的属性 **equivalentContent** 指示）有助于尽可能确保设备安全，并阻止设备在几天后收到快速更新，然后收到另一个 `latestSecurity` 定期更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-137">This behavior of offering the latest applicable update, indicated by the property **equivalentContent** being set to the default value `latestSecurity`, helps keep devices as secure as possible and prevents a device from receiving an expedited update followed by another regular update just days later.</span></span>

<span data-ttu-id="93fa1-138">可以使用部署用户体验设置中的 **属性 daysUntilForcedReboot** 配置 [设备重启](/graph/api/resources/windowsupdates-userexperiencesettings) 宽限期。</span><span class="sxs-lookup"><span data-stu-id="93fa1-138">You can configure the device restart grace period using the property **daysUntilForcedReboot** in the [user experience settings](/graph/api/resources/windowsupdates-userexperiencesettings) of the deployment.</span></span> <span data-ttu-id="93fa1-139">宽限期设置安装后用户可以控制设备重启时间的时间量。</span><span class="sxs-lookup"><span data-stu-id="93fa1-139">The grace period sets the amount of time after installation that the user can control the timing of when the device restarts.</span></span> <span data-ttu-id="93fa1-140">如果设备在宽限期到期时尚未重新启动，则会自动重新启动。</span><span class="sxs-lookup"><span data-stu-id="93fa1-140">If the device has not restarted by the time the grace period expires, it restarts automatically.</span></span>

<span data-ttu-id="93fa1-141">下面是为快速质量更新创建部署的示例。</span><span class="sxs-lookup"><span data-stu-id="93fa1-141">Below is an example of creating a deployment for an expedited quality update.</span></span> <span data-ttu-id="93fa1-142">目标设备在下一步中指定。</span><span class="sxs-lookup"><span data-stu-id="93fa1-142">The targeted devices are specified in the next step.</span></span>

### <a name="request"></a><span data-ttu-id="93fa1-143">请求</span><span class="sxs-lookup"><span data-stu-id="93fa1-143">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DD"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
        }
    }
}
```

### <a name="response"></a><span data-ttu-id="93fa1-144">响应</span><span class="sxs-lookup"><span data-stu-id="93fa1-144">Response</span></span>

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
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DDT00:00:00Z",
        "classification": "security",
        "equivalentContent": "latestSecurity"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
        },
        "monitoring": null,
        "rollout": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="93fa1-145">步骤 3：将设备分配给部署访问群体</span><span class="sxs-lookup"><span data-stu-id="93fa1-145">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="93fa1-146">创建部署后，你可以将设备分配给部署 [访问群体](/graph/api/resources/windowsupdates-deploymentaudience)。</span><span class="sxs-lookup"><span data-stu-id="93fa1-146">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="93fa1-147">成功更新部署访问群体后，Windows更新开始根据部署设置向相关设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-147">When the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="93fa1-148">在将设备添加到部署访问群体的成员或排除集合时 (会自动向服务注册设备 (也就是说，如果 [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) 对象) 。</span><span class="sxs-lookup"><span data-stu-id="93fa1-148">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (that is, an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="93fa1-149">以下示例演示如何将 Azure AD 设备添加为部署访问群体的成员。</span><span class="sxs-lookup"><span data-stu-id="93fa1-149">The following example shows how to add Azure AD devices as members of the deployment audience.</span></span>

### <a name="request"></a><span data-ttu-id="93fa1-150">请求</span><span class="sxs-lookup"><span data-stu-id="93fa1-150">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
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
    ]
}
```

### <a name="response"></a><span data-ttu-id="93fa1-151">响应</span><span class="sxs-lookup"><span data-stu-id="93fa1-151">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="93fa1-152">部署期间</span><span class="sxs-lookup"><span data-stu-id="93fa1-152">During a deployment</span></span>

<span data-ttu-id="93fa1-153">在部署过程中，可以通过更新部署的状态来暂停部署，也可以更新其访问群体成员和排除项。</span><span class="sxs-lookup"><span data-stu-id="93fa1-153">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="93fa1-154">部署后</span><span class="sxs-lookup"><span data-stu-id="93fa1-154">After a deployment</span></span>

<span data-ttu-id="93fa1-155">在最初向部署访问群体分配的所有设备都提供更新后，由于设备连接等因素，并非所有设备都启动或完成了更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-155">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="93fa1-156">只要部署仍然存在，它就会继续确保Windows只要重新连接，就会向分配的设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="93fa1-156">As long as the deployment still exists, it continues to make sure that Windows Update is offering the update to the assigned devices whenever they reconnect.</span></span>
