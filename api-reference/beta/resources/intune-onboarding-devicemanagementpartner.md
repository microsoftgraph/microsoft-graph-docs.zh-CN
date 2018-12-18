---
title: deviceManagementPartner 资源类型
description: 表示与设备管理合作伙伴的连接的实体。
author: tfitzmac
ms.openlocfilehash: 2174f81f7b9c5e73c3bc42a54cb030cf50c216d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354037"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="741b7-103">deviceManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="741b7-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="741b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="741b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="741b7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="741b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="741b7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="741b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="741b7-107">表示与设备管理合作伙伴的连接的实体。</span><span class="sxs-lookup"><span data-stu-id="741b7-107">Entity which represents a connection to device management partner.</span></span>
## <a name="methods"></a><span data-ttu-id="741b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="741b7-108">Methods</span></span>
|<span data-ttu-id="741b7-109">方法</span><span class="sxs-lookup"><span data-stu-id="741b7-109">Method</span></span>|<span data-ttu-id="741b7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="741b7-110">Return Type</span></span>|<span data-ttu-id="741b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="741b7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="741b7-112">列出 deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="741b7-112">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="741b7-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="741b7-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="741b7-114">列出 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="741b7-114">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="741b7-115">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-115">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="741b7-116">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-116">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="741b7-117">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="741b7-117">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="741b7-118">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-118">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="741b7-119">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-119">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="741b7-120">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="741b7-120">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="741b7-121">删除 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-121">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="741b7-122">无</span><span class="sxs-lookup"><span data-stu-id="741b7-122">None</span></span>|<span data-ttu-id="741b7-123">删除 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="741b7-123">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="741b7-124">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-124">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="741b7-125">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="741b7-125">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="741b7-126">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="741b7-126">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="741b7-127">属性</span><span class="sxs-lookup"><span data-stu-id="741b7-127">Properties</span></span>
|<span data-ttu-id="741b7-128">属性</span><span class="sxs-lookup"><span data-stu-id="741b7-128">Property</span></span>|<span data-ttu-id="741b7-129">类型</span><span class="sxs-lookup"><span data-stu-id="741b7-129">Type</span></span>|<span data-ttu-id="741b7-130">说明</span><span class="sxs-lookup"><span data-stu-id="741b7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="741b7-131">id</span><span class="sxs-lookup"><span data-stu-id="741b7-131">id</span></span>|<span data-ttu-id="741b7-132">字符串</span><span class="sxs-lookup"><span data-stu-id="741b7-132">String</span></span>|<span data-ttu-id="741b7-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="741b7-133">Not yet documented</span></span>|
|<span data-ttu-id="741b7-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="741b7-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="741b7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741b7-135">DateTimeOffset</span></span>|<span data-ttu-id="741b7-136">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="741b7-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="741b7-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="741b7-137">partnerState</span></span>|[<span data-ttu-id="741b7-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="741b7-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="741b7-139">合作伙伴的此租户的状态。</span><span class="sxs-lookup"><span data-stu-id="741b7-139">Partner state of this tenant.</span></span> <span data-ttu-id="741b7-140">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="741b7-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="741b7-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="741b7-141">partnerAppType</span></span>|[<span data-ttu-id="741b7-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="741b7-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="741b7-143">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="741b7-143">Partner App type.</span></span> <span data-ttu-id="741b7-144">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="741b7-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="741b7-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="741b7-145">singleTenantAppId</span></span>|<span data-ttu-id="741b7-146">String</span><span class="sxs-lookup"><span data-stu-id="741b7-146">String</span></span>|<span data-ttu-id="741b7-147">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="741b7-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="741b7-148">displayName</span><span class="sxs-lookup"><span data-stu-id="741b7-148">displayName</span></span>|<span data-ttu-id="741b7-149">String</span><span class="sxs-lookup"><span data-stu-id="741b7-149">String</span></span>|<span data-ttu-id="741b7-150">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="741b7-150">Partner display name</span></span>|
|<span data-ttu-id="741b7-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="741b7-151">isConfigured</span></span>|<span data-ttu-id="741b7-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="741b7-152">Boolean</span></span>|<span data-ttu-id="741b7-153">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="741b7-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="741b7-154">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="741b7-154">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="741b7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741b7-155">DateTimeOffset</span></span>|<span data-ttu-id="741b7-156">采用 UTC 时将删除 PartnerDevices 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="741b7-156">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="741b7-157">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="741b7-157">This will become obselete soon.</span></span>|
|<span data-ttu-id="741b7-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="741b7-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="741b7-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741b7-159">DateTimeOffset</span></span>|<span data-ttu-id="741b7-160">采用 UTC PartnerDevices 将标记为不符合时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="741b7-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="741b7-161">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="741b7-161">This will become obselete soon.</span></span>|
|<span data-ttu-id="741b7-162">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="741b7-162">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="741b7-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741b7-163">DateTimeOffset</span></span>|<span data-ttu-id="741b7-164">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="741b7-164">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="741b7-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="741b7-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="741b7-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741b7-166">DateTimeOffset</span></span>|<span data-ttu-id="741b7-167">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="741b7-167">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="741b7-168">关系</span><span class="sxs-lookup"><span data-stu-id="741b7-168">Relationships</span></span>
<span data-ttu-id="741b7-169">无</span><span class="sxs-lookup"><span data-stu-id="741b7-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="741b7-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="741b7-170">JSON Representation</span></span>
<span data-ttu-id="741b7-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="741b7-171">Here is a JSON representation of the resource.</span></span>
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





