---
title: Windows Update for Business 部署服务中的部署
description: 部署是 Windows Update for Business 部署服务的基础。 通过部署，你可以将一组设备作为目标，以从 Windows 更新（如软件更新）接收特定内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 74cf9f7082d2f7d69f60a8edf851c881a59a67aa
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067665"
---
# <a name="deployments-in-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="c2b64-104">Windows Update for Business 部署服务中的部署</span><span class="sxs-lookup"><span data-stu-id="c2b64-104">Deployments in the Windows Update for Business deployment service</span></span>

<span data-ttu-id="c2b64-105">部署是 Windows Update for Business 部署服务的基础。</span><span class="sxs-lookup"><span data-stu-id="c2b64-105">Deployments are the foundation of the Windows Update for Business deployment service.</span></span> <span data-ttu-id="c2b64-106">通过部署，你可以面向一组设备，以接收来自 Windows Update 的特定内容，例如[软件更新](windowsupdates-software-updates.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b64-106">Through a deployment you can target a set of devices to receive specific content from Windows Update, such as a [software update](windowsupdates-software-updates.md).</span></span>

<span data-ttu-id="c2b64-107">部署具有以下主要方面：</span><span class="sxs-lookup"><span data-stu-id="c2b64-107">Deployments have the following key aspects:</span></span>

1. <span data-ttu-id="c2b64-108">内容：可从目录部署的更新。</span><span class="sxs-lookup"><span data-stu-id="c2b64-108">Content: The update available to deploy from the catalog.</span></span> <span data-ttu-id="c2b64-109">这由 [deployableContent](/graph/api/resources/windowsupdates-deployablecontent)**类型的** content 属性表示。</span><span class="sxs-lookup"><span data-stu-id="c2b64-109">This is represented by the **content** property of the [deployableContent](/graph/api/resources/windowsupdates-deployablecontent) type.</span></span>
2. <span data-ttu-id="c2b64-110">访问群体：用于接收内容的设备。</span><span class="sxs-lookup"><span data-stu-id="c2b64-110">Audience: The devices to receive content.</span></span> <span data-ttu-id="c2b64-111">这是[deploymentAudience 类型的访问群体](/graph/api/resources/windowsupdates-deploymentaudience)关系。 </span><span class="sxs-lookup"><span data-stu-id="c2b64-111">This is an **audience** relationship of the [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) type.</span></span>
3. <span data-ttu-id="c2b64-112">设置：管理内容传递到设备的方式和时间的设置。</span><span class="sxs-lookup"><span data-stu-id="c2b64-112">Settings: The settings governing how and when content should be delivered to devices.</span></span> <span data-ttu-id="c2b64-113">这由 [deploymentSettings](/graph/api/resources/windowsupdates-deploymentsettings)类型的 **settings** 属性表示。</span><span class="sxs-lookup"><span data-stu-id="c2b64-113">This is represented by the **settings** property of the [deploymentSettings](/graph/api/resources/windowsupdates-deploymentsettings) type.</span></span>
4. <span data-ttu-id="c2b64-114">状态：部署在其生命周期中的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c2b64-114">State: The current state of the deployment within its lifecycle.</span></span> <span data-ttu-id="c2b64-115">这由 [deploymentState](/graph/api/resources/windowsupdates-deploymentstate)类型的 **state** 属性表示。</span><span class="sxs-lookup"><span data-stu-id="c2b64-115">This is represented by the **state** property of the [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) type.</span></span>

## <a name="create-a-deployment-with-content-and-an-audience"></a><span data-ttu-id="c2b64-116">创建包含内容和访问群体部署的部署</span><span class="sxs-lookup"><span data-stu-id="c2b64-116">Create a deployment with content and an audience</span></span>


<span data-ttu-id="c2b64-117">由于内容和访问群体是定义部署的关键，因此在创建时必须同时分配这两者。</span><span class="sxs-lookup"><span data-stu-id="c2b64-117">Because content and audience are key to the definition of a deployment, you are required to assign both at the time of creation.</span></span> <span data-ttu-id="c2b64-118">尽管以后无法更改内容和访问群体分配，但访问群体中的设备成员身份可以。</span><span class="sxs-lookup"><span data-stu-id="c2b64-118">While content and audience assignments cannot be changed later, device membership within an audience can.</span></span>

<span data-ttu-id="c2b64-119">若要详细了解如何创建部署，请参阅 [部署功能更新](windowsupdates-deploy-update.md) 和 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b64-119">To learn more about creating a deployment, see [Deploy a feature update](windowsupdates-deploy-update.md) and [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

## <a name="configure-settings"></a><span data-ttu-id="c2b64-120">配置设置</span><span class="sxs-lookup"><span data-stu-id="c2b64-120">Configure settings</span></span>

### <a name="rollout"></a><span data-ttu-id="c2b64-121">推出</span><span class="sxs-lookup"><span data-stu-id="c2b64-121">Rollout</span></span>

<span data-ttu-id="c2b64-122">[推出](/graph/api/resources/windowsupdates-rolloutsettings) 设置控制内容在一段时间之后如何部署到部署访问群体中的设备。</span><span class="sxs-lookup"><span data-stu-id="c2b64-122">[Rollout settings](/graph/api/resources/windowsupdates-rolloutsettings) govern how the content is deployed over time to devices in the deployment audience.</span></span> <span data-ttu-id="c2b64-123">你可以为部署功能更新配置推出设置。</span><span class="sxs-lookup"><span data-stu-id="c2b64-123">You can configure rollout settings for deployments of feature updates.</span></span>

<span data-ttu-id="c2b64-124">若要了解有关推出设置的信息，请参阅计划 [部署](windowsupdates-schedule-deployment.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b64-124">To learn more about rollout settings, see [Schedule a deployment](windowsupdates-schedule-deployment.md).</span></span>

### <a name="monitoring"></a><span data-ttu-id="c2b64-125">监控</span><span class="sxs-lookup"><span data-stu-id="c2b64-125">Monitoring</span></span>

<span data-ttu-id="c2b64-126">可以使用监视 [设置](/graph/api/resources/windowsupdates-monitoringsettings) 来配置警报，并基于来自设备的更新信号自动执行操作。</span><span class="sxs-lookup"><span data-stu-id="c2b64-126">You can use [monitoring settings](/graph/api/resources/windowsupdates-monitoringsettings) to configure alerts and automated actions to take based on update signals from devices.</span></span> <span data-ttu-id="c2b64-127">可以针对功能更新的部署配置监视设置。</span><span class="sxs-lookup"><span data-stu-id="c2b64-127">Monitoring settings can be configured for deployments of feature updates.</span></span>


<span data-ttu-id="c2b64-128">若要了解有关监视设置的信息，请参阅 [管理监视规则](windowsupdates-manage-monitoring-rules.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b64-128">To learn more about monitoring settings, see [Manage monitoring rules](windowsupdates-manage-monitoring-rules.md).</span></span>

### <a name="user-experience"></a><span data-ttu-id="c2b64-129">用户体验</span><span class="sxs-lookup"><span data-stu-id="c2b64-129">User experience</span></span>

<span data-ttu-id="c2b64-130">对于快速质量更新的部署， [用户体验设置](/graph/api/resources/windowsupdates-userexperiencesettings) 会临时替代设备上现有的策略，以便获得更新体验。</span><span class="sxs-lookup"><span data-stu-id="c2b64-130">For deployments of expedited quality updates, [user experience settings](/graph/api/resources/windowsupdates-userexperiencesettings) temporarily override existing policies on the device for update experience.</span></span>

<span data-ttu-id="c2b64-131">若要了解有关用户体验设置的信息，请参阅 [部署加速安全更新](windowsupdates-deploy-expedited-update.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b64-131">To learn more about user experience settings, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

## <a name="get-or-set-lifecycle-state"></a><span data-ttu-id="c2b64-132">获取或设置生命周期状态</span><span class="sxs-lookup"><span data-stu-id="c2b64-132">Get or set lifecycle state</span></span>

### <a name="states"></a><span data-ttu-id="c2b64-133">状态</span><span class="sxs-lookup"><span data-stu-id="c2b64-133">States</span></span>

<span data-ttu-id="c2b64-134">部署在生命周期状态中移动，如下表所述。</span><span class="sxs-lookup"><span data-stu-id="c2b64-134">Deployments move through lifecycle states as described in the following table.</span></span>

| <span data-ttu-id="c2b64-135">状态</span><span class="sxs-lookup"><span data-stu-id="c2b64-135">State</span></span>     | <span data-ttu-id="c2b64-136">说明</span><span class="sxs-lookup"><span data-stu-id="c2b64-136">Description</span></span>                                                                                       |
|-----------|---------------------------------------------------------------------------------------------------|
| `scheduled` | <span data-ttu-id="c2b64-137">部署正在等待满足产品/服务条件，以开始向设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="c2b64-137">The deployment is waiting for offer conditions to be met to start offering the update to devices.</span></span> |
| `offering`  | <span data-ttu-id="c2b64-138">部署正在向设备提供更新。</span><span class="sxs-lookup"><span data-stu-id="c2b64-138">The deployment is offering the update to devices.</span></span>                                                 |
| `paused`    | <span data-ttu-id="c2b64-139">部署将暂停，并阻止向设备提供更新，直到未暂停。</span><span class="sxs-lookup"><span data-stu-id="c2b64-139">The deployment is paused and prevented from offering the update to devices until it is unpaused.</span></span>  |


### <a name="transitions"></a><span data-ttu-id="c2b64-140">Transitions</span><span class="sxs-lookup"><span data-stu-id="c2b64-140">Transitions</span></span>

| <span data-ttu-id="c2b64-141">Transition</span><span class="sxs-lookup"><span data-stu-id="c2b64-141">Transition</span></span>                     | <span data-ttu-id="c2b64-142">Condition</span><span class="sxs-lookup"><span data-stu-id="c2b64-142">Condition</span></span>                                |
|--------------------------------|------------------------------------------|
| <span data-ttu-id="c2b64-143">`scheduled` → `offering`</span><span class="sxs-lookup"><span data-stu-id="c2b64-143">`scheduled` → `offering`</span></span>           | <span data-ttu-id="c2b64-144">满足计划条件。</span><span class="sxs-lookup"><span data-stu-id="c2b64-144">Scheduling condition is met.</span></span>             |
| <span data-ttu-id="c2b64-145">`offering` → `scheduled`</span><span class="sxs-lookup"><span data-stu-id="c2b64-145">`offering` → `scheduled`</span></span>           | <span data-ttu-id="c2b64-146">不满足计划条件。</span><span class="sxs-lookup"><span data-stu-id="c2b64-146">Scheduling condition is not met.</span></span>         |
| <span data-ttu-id="c2b64-147">`scheduled` 或 `offering` → `paused`</span><span class="sxs-lookup"><span data-stu-id="c2b64-147">`scheduled` or `offering` → `paused`</span></span> | <span data-ttu-id="c2b64-148">有一个暂停的请求或自动操作。</span><span class="sxs-lookup"><span data-stu-id="c2b64-148">There is a request or automatic action to pause.</span></span> |
| <span data-ttu-id="c2b64-149">`paused` → `scheduled` 或 `offering`</span><span class="sxs-lookup"><span data-stu-id="c2b64-149">`paused` → `scheduled` or `offering`</span></span> | <span data-ttu-id="c2b64-150">不再有要暂停的请求或自动操作。</span><span class="sxs-lookup"><span data-stu-id="c2b64-150">There is no longer a request or automatic action to pause.</span></span> |

### <a name="resource-model"></a><span data-ttu-id="c2b64-151">资源模型</span><span class="sxs-lookup"><span data-stu-id="c2b64-151">Resource model</span></span>

<span data-ttu-id="c2b64-152">部署 [资源](/graph/api/resources/windowsupdates-deployment)具有 [deploymentState](/graph/api/resources/windowsupdates-deploymentstate)类型的 **state** 属性，该属性提供有关当前生命周期状态的信息。</span><span class="sxs-lookup"><span data-stu-id="c2b64-152">The [deployment](/graph/api/resources/windowsupdates-deployment) resource has a **state** property of type [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) which provides information about the current lifecycle state.</span></span>

<span data-ttu-id="c2b64-153">该服务确定部署 **状态** 的有效值作为多个输入和异步进程的结果，但可以通过将 **requestedValue** 设置为这些输入之一来请求特定值。</span><span class="sxs-lookup"><span data-stu-id="c2b64-153">The service determines the effective **value** of the deployment state as a net result of several inputs and asynchronous processes, but you can request a particular value by setting **requestedValue** as one of these inputs.</span></span> <span data-ttu-id="c2b64-154">有效部署状态值的其他输入包括推出设置和监视设置。</span><span class="sxs-lookup"><span data-stu-id="c2b64-154">Other inputs to the effective deployment state value include rollout settings and monitoring settings.</span></span>

## <a name="multiple-deployments"></a><span data-ttu-id="c2b64-155">多个部署</span><span class="sxs-lookup"><span data-stu-id="c2b64-155">Multiple deployments</span></span>

<span data-ttu-id="c2b64-156">你可以一次将设备分配给多个部署。</span><span class="sxs-lookup"><span data-stu-id="c2b64-156">You can assign a device to multiple deployments at one time.</span></span> <span data-ttu-id="c2b64-157">这些部署可用于相同更新类别的内容 (例如，所有部署都是功能更新) ，或用于不同更新类别的内容。</span><span class="sxs-lookup"><span data-stu-id="c2b64-157">These deployments can be for content of the same update category (for example all deployments are feature updates), or for content of different update categories.</span></span>

<span data-ttu-id="c2b64-158">为不同更新类别的内容分配设备 (例如功能更新和快速质量更新) 时，部署服务根据 Microsoft 的建议按顺序提供内容。</span><span class="sxs-lookup"><span data-stu-id="c2b64-158">When you assign a device to two deployments for content of different update categories (for example, a feature update and an expedited quality update), the deployment service offers content in a sequence according to Microsoft’s recommendation.</span></span>

<span data-ttu-id="c2b64-159">为同一更新类别 (的内容分配设备时 (例如，功能更新版本 20H1 和 20H2，或 2021 年 3 月和 2021 年 4 月的质量更新) 部署服务会提供 Microsoft 排名更高的内容。</span><span class="sxs-lookup"><span data-stu-id="c2b64-159">When you assign a device to two deployments for content of the same update category (for example, feature update versions 20H1 and 20H2, or quality updates from March 2021 and April 2021), the deployment service offers the content that is higher ranked by Microsoft.</span></span> <span data-ttu-id="c2b64-160">对于功能更新和质量更新，最新更新的排名更高。</span><span class="sxs-lookup"><span data-stu-id="c2b64-160">For feature updates and quality updates, more recent updates are higher ranked.</span></span> <span data-ttu-id="c2b64-161">如果其中一个部署仍为设备计划，并且尚未准备好提供内容，则此行为不适用。</span><span class="sxs-lookup"><span data-stu-id="c2b64-161">This behavior does not apply if one of the deployments is still scheduled for the device and is not ready to offer content.</span></span> <span data-ttu-id="c2b64-162">在这种情况下，其他部署将内容交付到设备。</span><span class="sxs-lookup"><span data-stu-id="c2b64-162">In that case, the other deployment delivers content to the device.</span></span>
