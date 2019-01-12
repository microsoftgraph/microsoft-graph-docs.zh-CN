---
title: managedDeviceMobileAppConfigurationDeviceStatus 资源类型
description: 包含的属性、 继承的属性和设备 MDM 移动应用程序配置状态的操作。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 43bc21430bb6e03f5e8503b1efe9fbae306fcffd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947867"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a><span data-ttu-id="d4876-103">managedDeviceMobileAppConfigurationDeviceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4876-103">managedDeviceMobileAppConfigurationDeviceStatus resource type</span></span>

> <span data-ttu-id="d4876-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4876-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4876-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4876-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4876-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d4876-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4876-107">包含的属性、 继承的属性和设备 MDM 移动应用程序配置状态的操作。</span><span class="sxs-lookup"><span data-stu-id="d4876-107">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="d4876-108">方法</span><span class="sxs-lookup"><span data-stu-id="d4876-108">Methods</span></span>
|<span data-ttu-id="d4876-109">方法</span><span class="sxs-lookup"><span data-stu-id="d4876-109">Method</span></span>|<span data-ttu-id="d4876-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4876-110">Return Type</span></span>|<span data-ttu-id="d4876-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4876-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4876-112">列表 managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d4876-112">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|<span data-ttu-id="d4876-113">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="d4876-113">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d4876-114">列出属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d4876-114">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>|
|[<span data-ttu-id="d4876-115">获取 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-115">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[<span data-ttu-id="d4876-116">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-116">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="d4876-117">读取属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d4876-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="d4876-118">创建 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-118">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[<span data-ttu-id="d4876-119">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-119">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="d4876-120">创建新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4876-120">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="d4876-121">删除 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-121">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|<span data-ttu-id="d4876-122">无</span><span class="sxs-lookup"><span data-stu-id="d4876-122">None</span></span>|<span data-ttu-id="d4876-123">删除[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="d4876-123">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>|
|[<span data-ttu-id="d4876-124">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-124">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[<span data-ttu-id="d4876-125">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-125">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="d4876-126">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d4876-126">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4876-127">属性</span><span class="sxs-lookup"><span data-stu-id="d4876-127">Properties</span></span>
|<span data-ttu-id="d4876-128">属性</span><span class="sxs-lookup"><span data-stu-id="d4876-128">Property</span></span>|<span data-ttu-id="d4876-129">类型</span><span class="sxs-lookup"><span data-stu-id="d4876-129">Type</span></span>|<span data-ttu-id="d4876-130">说明</span><span class="sxs-lookup"><span data-stu-id="d4876-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4876-131">id</span><span class="sxs-lookup"><span data-stu-id="d4876-131">id</span></span>|<span data-ttu-id="d4876-132">String</span><span class="sxs-lookup"><span data-stu-id="d4876-132">String</span></span>|<span data-ttu-id="d4876-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d4876-133">Key of the entity.</span></span>|
|<span data-ttu-id="d4876-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d4876-134">deviceDisplayName</span></span>|<span data-ttu-id="d4876-135">String</span><span class="sxs-lookup"><span data-stu-id="d4876-135">String</span></span>|<span data-ttu-id="d4876-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="d4876-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d4876-137">userName</span><span class="sxs-lookup"><span data-stu-id="d4876-137">userName</span></span>|<span data-ttu-id="d4876-138">String</span><span class="sxs-lookup"><span data-stu-id="d4876-138">String</span></span>|<span data-ttu-id="d4876-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="d4876-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="d4876-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d4876-140">deviceModel</span></span>|<span data-ttu-id="d4876-141">String</span><span class="sxs-lookup"><span data-stu-id="d4876-141">String</span></span>|<span data-ttu-id="d4876-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="d4876-142">The device model that is being reported</span></span>|
|<span data-ttu-id="d4876-143">platform</span><span class="sxs-lookup"><span data-stu-id="d4876-143">platform</span></span>|<span data-ttu-id="d4876-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d4876-144">Int32</span></span>|<span data-ttu-id="d4876-145">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="d4876-145">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="d4876-146">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d4876-146">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d4876-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4876-147">DateTimeOffset</span></span>|<span data-ttu-id="d4876-148">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d4876-148">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d4876-149">status</span><span class="sxs-lookup"><span data-stu-id="d4876-149">status</span></span>|[<span data-ttu-id="d4876-150">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d4876-150">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d4876-151">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d4876-151">Compliance status of the policy report.</span></span> <span data-ttu-id="d4876-152">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d4876-152">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d4876-153">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4876-153">lastReportedDateTime</span></span>|<span data-ttu-id="d4876-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4876-154">DateTimeOffset</span></span>|<span data-ttu-id="d4876-155">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="d4876-155">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d4876-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4876-156">userPrincipalName</span></span>|<span data-ttu-id="d4876-157">String</span><span class="sxs-lookup"><span data-stu-id="d4876-157">String</span></span>|<span data-ttu-id="d4876-158">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d4876-158">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4876-159">关系</span><span class="sxs-lookup"><span data-stu-id="d4876-159">Relationships</span></span>
<span data-ttu-id="d4876-160">无</span><span class="sxs-lookup"><span data-stu-id="d4876-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d4876-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4876-161">JSON Representation</span></span>
<span data-ttu-id="d4876-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4876-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





