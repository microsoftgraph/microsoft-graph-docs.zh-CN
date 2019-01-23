---
title: deviceManagementPartner 资源类型
description: 表示与设备管理合作伙伴的连接的实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 87c01360f07d3a7257dbd417a27d16ab674c8989
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398399"
---
# <a name="devicemanagementpartner-resource-type"></a><span data-ttu-id="064ec-103">deviceManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="064ec-103">deviceManagementPartner resource type</span></span>

> <span data-ttu-id="064ec-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="064ec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="064ec-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="064ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="064ec-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="064ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="064ec-107">表示与设备管理合作伙伴的连接的实体。</span><span class="sxs-lookup"><span data-stu-id="064ec-107">Entity which represents a connection to device management partner.</span></span>

## <a name="methods"></a><span data-ttu-id="064ec-108">方法</span><span class="sxs-lookup"><span data-stu-id="064ec-108">Methods</span></span>
|<span data-ttu-id="064ec-109">方法</span><span class="sxs-lookup"><span data-stu-id="064ec-109">Method</span></span>|<span data-ttu-id="064ec-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="064ec-110">Return Type</span></span>|<span data-ttu-id="064ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="064ec-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="064ec-112">列出 deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="064ec-112">List deviceManagementPartners</span></span>](../api/intune-onboarding-devicemanagementpartner-list.md)|<span data-ttu-id="064ec-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="064ec-113">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="064ec-114">列出 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="064ec-114">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="064ec-115">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-115">Get deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-get.md)|[<span data-ttu-id="064ec-116">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-116">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="064ec-117">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="064ec-117">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="064ec-118">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-118">Create deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-create.md)|[<span data-ttu-id="064ec-119">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-119">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="064ec-120">创建新的 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="064ec-120">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="064ec-121">删除 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-121">Delete deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-delete.md)|<span data-ttu-id="064ec-122">无</span><span class="sxs-lookup"><span data-stu-id="064ec-122">None</span></span>|<span data-ttu-id="064ec-123">删除 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="064ec-123">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>|
|[<span data-ttu-id="064ec-124">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-124">Update deviceManagementPartner</span></span>](../api/intune-onboarding-devicemanagementpartner-update.md)|[<span data-ttu-id="064ec-125">deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="064ec-125">deviceManagementPartner</span></span>](../resources/intune-onboarding-devicemanagementpartner.md)|<span data-ttu-id="064ec-126">更新 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="064ec-126">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="064ec-127">属性</span><span class="sxs-lookup"><span data-stu-id="064ec-127">Properties</span></span>
|<span data-ttu-id="064ec-128">属性</span><span class="sxs-lookup"><span data-stu-id="064ec-128">Property</span></span>|<span data-ttu-id="064ec-129">类型</span><span class="sxs-lookup"><span data-stu-id="064ec-129">Type</span></span>|<span data-ttu-id="064ec-130">说明</span><span class="sxs-lookup"><span data-stu-id="064ec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="064ec-131">id</span><span class="sxs-lookup"><span data-stu-id="064ec-131">id</span></span>|<span data-ttu-id="064ec-132">String</span><span class="sxs-lookup"><span data-stu-id="064ec-132">String</span></span>|<span data-ttu-id="064ec-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="064ec-133">Not yet documented</span></span>|
|<span data-ttu-id="064ec-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="064ec-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="064ec-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="064ec-135">DateTimeOffset</span></span>|<span data-ttu-id="064ec-136">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="064ec-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="064ec-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="064ec-137">partnerState</span></span>|[<span data-ttu-id="064ec-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="064ec-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="064ec-139">合作伙伴的此租户的状态。</span><span class="sxs-lookup"><span data-stu-id="064ec-139">Partner state of this tenant.</span></span> <span data-ttu-id="064ec-140">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="064ec-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="064ec-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="064ec-141">partnerAppType</span></span>|[<span data-ttu-id="064ec-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="064ec-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="064ec-143">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="064ec-143">Partner App type.</span></span> <span data-ttu-id="064ec-144">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="064ec-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="064ec-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="064ec-145">singleTenantAppId</span></span>|<span data-ttu-id="064ec-146">String</span><span class="sxs-lookup"><span data-stu-id="064ec-146">String</span></span>|<span data-ttu-id="064ec-147">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="064ec-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="064ec-148">displayName</span><span class="sxs-lookup"><span data-stu-id="064ec-148">displayName</span></span>|<span data-ttu-id="064ec-149">String</span><span class="sxs-lookup"><span data-stu-id="064ec-149">String</span></span>|<span data-ttu-id="064ec-150">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="064ec-150">Partner display name</span></span>|
|<span data-ttu-id="064ec-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="064ec-151">isConfigured</span></span>|<span data-ttu-id="064ec-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="064ec-152">Boolean</span></span>|<span data-ttu-id="064ec-153">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="064ec-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="064ec-154">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="064ec-154">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="064ec-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="064ec-155">DateTimeOffset</span></span>|<span data-ttu-id="064ec-156">采用 UTC 时将删除 PartnerDevices 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="064ec-156">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="064ec-157">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="064ec-157">This will become obselete soon.</span></span>|
|<span data-ttu-id="064ec-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="064ec-158">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="064ec-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="064ec-159">DateTimeOffset</span></span>|<span data-ttu-id="064ec-160">采用 UTC PartnerDevices 将标记为不符合时的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="064ec-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="064ec-161">这将立即成为过时。</span><span class="sxs-lookup"><span data-stu-id="064ec-161">This will become obselete soon.</span></span>|
|<span data-ttu-id="064ec-162">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="064ec-162">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="064ec-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="064ec-163">DateTimeOffset</span></span>|<span data-ttu-id="064ec-164">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="064ec-164">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="064ec-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="064ec-165">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="064ec-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="064ec-166">DateTimeOffset</span></span>|<span data-ttu-id="064ec-167">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="064ec-167">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|

## <a name="relationships"></a><span data-ttu-id="064ec-168">关系</span><span class="sxs-lookup"><span data-stu-id="064ec-168">Relationships</span></span>
<span data-ttu-id="064ec-169">无</span><span class="sxs-lookup"><span data-stu-id="064ec-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="064ec-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="064ec-170">JSON Representation</span></span>
<span data-ttu-id="064ec-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="064ec-171">Here is a JSON representation of the resource.</span></span>
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




