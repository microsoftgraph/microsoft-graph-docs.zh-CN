---
title: deviceManagementPartner 资源类型
description: 表示与设备管理合作伙伴的连接的实体。
ms.openlocfilehash: c682b700636ad80f20719e40f35a929cf740c7a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048260"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="31a04-103">deviceManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="31a04-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="31a04-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="31a04-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31a04-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="31a04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31a04-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="31a04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31a04-107">表示与设备管理合作伙伴的连接的实体。</span><span class="sxs-lookup"><span data-stu-id="31a04-107">Entity which represents a connection to device management partner.</span></span>
## <a name="methods"></a><span data-ttu-id="31a04-108">方法</span><span class="sxs-lookup"><span data-stu-id="31a04-108">Methods</span></span>
|<span data-ttu-id="31a04-109">方法</span><span class="sxs-lookup"><span data-stu-id="31a04-109">Method</span></span>|<span data-ttu-id="31a04-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="31a04-110">Return Type</span></span>|<span data-ttu-id="31a04-111">说明</span><span class="sxs-lookup"><span data-stu-id="31a04-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31a04-112">列出 deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="31a04-112">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="31a04-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31a04-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="31a04-114">列出 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31a04-114">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="31a04-115">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-115">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="31a04-116">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-116">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="31a04-117">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31a04-117">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="31a04-118">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-118">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="31a04-119">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-119">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="31a04-120">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31a04-120">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="31a04-121">删除 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-121">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="31a04-122">无</span><span class="sxs-lookup"><span data-stu-id="31a04-122">None</span></span>|<span data-ttu-id="31a04-123">删除 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="31a04-123">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="31a04-124">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-124">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="31a04-125">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="31a04-125">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="31a04-126">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="31a04-126">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31a04-127">属性</span><span class="sxs-lookup"><span data-stu-id="31a04-127">Properties</span></span>
|<span data-ttu-id="31a04-128">属性</span><span class="sxs-lookup"><span data-stu-id="31a04-128">Property</span></span>|<span data-ttu-id="31a04-129">类型</span><span class="sxs-lookup"><span data-stu-id="31a04-129">Type</span></span>|<span data-ttu-id="31a04-130">说明</span><span class="sxs-lookup"><span data-stu-id="31a04-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a04-131">id</span><span class="sxs-lookup"><span data-stu-id="31a04-131">id</span></span>|<span data-ttu-id="31a04-132">字符串</span><span class="sxs-lookup"><span data-stu-id="31a04-132">String</span></span>|<span data-ttu-id="31a04-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31a04-133">Not yet documented</span></span>|
|<span data-ttu-id="31a04-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="31a04-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="31a04-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31a04-135">DateTimeOffset</span></span>|<span data-ttu-id="31a04-136">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="31a04-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="31a04-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="31a04-137">partnerState</span></span>|[<span data-ttu-id="31a04-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="31a04-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="31a04-139">合作伙伴的此租户的状态。</span><span class="sxs-lookup"><span data-stu-id="31a04-139">Partner state of this tenant.</span></span> <span data-ttu-id="31a04-140">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="31a04-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="31a04-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="31a04-141">partnerAppType</span></span>|[<span data-ttu-id="31a04-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="31a04-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="31a04-143">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="31a04-143">Partner App type.</span></span> <span data-ttu-id="31a04-144">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="31a04-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="31a04-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="31a04-145">singleTenantAppId</span></span>|<span data-ttu-id="31a04-146">String</span><span class="sxs-lookup"><span data-stu-id="31a04-146">String</span></span>|<span data-ttu-id="31a04-147">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="31a04-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="31a04-148">displayName</span><span class="sxs-lookup"><span data-stu-id="31a04-148">displayName</span></span>|<span data-ttu-id="31a04-149">String</span><span class="sxs-lookup"><span data-stu-id="31a04-149">String</span></span>|<span data-ttu-id="31a04-150">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="31a04-150">Partner display name</span></span>|
|<span data-ttu-id="31a04-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="31a04-151">isConfigured</span></span>|<span data-ttu-id="31a04-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="31a04-152">Boolean</span></span>|<span data-ttu-id="31a04-153">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="31a04-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="31a04-154">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="31a04-154">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="31a04-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31a04-155">DateTimeOffset</span></span>|<span data-ttu-id="31a04-156">采用 UTC 时将删除 PartnerDevices 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31a04-156">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="31a04-157">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="31a04-157">This will become obselete soon.</span></span>|
|<span data-ttu-id="31a04-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="31a04-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="31a04-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31a04-159">DateTimeOffset</span></span>|<span data-ttu-id="31a04-160">采用 UTC PartnerDevices 将标记为不符合时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31a04-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="31a04-161">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="31a04-161">This will become obselete soon.</span></span>|
|<span data-ttu-id="31a04-162">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="31a04-162">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="31a04-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31a04-163">DateTimeOffset</span></span>|<span data-ttu-id="31a04-164">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="31a04-164">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="31a04-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="31a04-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="31a04-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31a04-166">DateTimeOffset</span></span>|<span data-ttu-id="31a04-167">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="31a04-167">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="31a04-168">关系</span><span class="sxs-lookup"><span data-stu-id="31a04-168">Relationships</span></span>
<span data-ttu-id="31a04-169">无</span><span class="sxs-lookup"><span data-stu-id="31a04-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31a04-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31a04-170">JSON Representation</span></span>
<span data-ttu-id="31a04-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31a04-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```





