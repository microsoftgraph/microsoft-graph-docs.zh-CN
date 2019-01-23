---
title: restrictedAppsViolation 资源类型
description: 与每个每个用户的设备的受限的应用程序配置文件的冲突
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcbd7def59d17dcd6e906e1e6bef85e3a448b880
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424978"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="35d6f-103">restrictedAppsViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d6f-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="35d6f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="35d6f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35d6f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="35d6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35d6f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35d6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d6f-107">与每个每个用户的设备的受限的应用程序配置文件的冲突</span><span class="sxs-lookup"><span data-stu-id="35d6f-107">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="35d6f-108">方法</span><span class="sxs-lookup"><span data-stu-id="35d6f-108">Methods</span></span>
|<span data-ttu-id="35d6f-109">方法</span><span class="sxs-lookup"><span data-stu-id="35d6f-109">Method</span></span>|<span data-ttu-id="35d6f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="35d6f-110">Return Type</span></span>|<span data-ttu-id="35d6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="35d6f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35d6f-112">列表 restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="35d6f-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="35d6f-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d6f-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="35d6f-114">列出属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="35d6f-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="35d6f-115">获取 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="35d6f-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="35d6f-117">读取属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="35d6f-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="35d6f-118">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="35d6f-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="35d6f-120">创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35d6f-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="35d6f-121">删除 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="35d6f-122">无</span><span class="sxs-lookup"><span data-stu-id="35d6f-122">None</span></span>|<span data-ttu-id="35d6f-123">删除[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。</span><span class="sxs-lookup"><span data-stu-id="35d6f-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="35d6f-124">更新 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="35d6f-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="35d6f-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="35d6f-126">更新[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35d6f-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35d6f-127">属性</span><span class="sxs-lookup"><span data-stu-id="35d6f-127">Properties</span></span>
|<span data-ttu-id="35d6f-128">属性</span><span class="sxs-lookup"><span data-stu-id="35d6f-128">Property</span></span>|<span data-ttu-id="35d6f-129">类型</span><span class="sxs-lookup"><span data-stu-id="35d6f-129">Type</span></span>|<span data-ttu-id="35d6f-130">说明</span><span class="sxs-lookup"><span data-stu-id="35d6f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d6f-131">id</span><span class="sxs-lookup"><span data-stu-id="35d6f-131">id</span></span>|<span data-ttu-id="35d6f-132">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-132">String</span></span>|<span data-ttu-id="35d6f-133">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="35d6f-133">Unique identifier for the object.</span></span> <span data-ttu-id="35d6f-134">由 accountId、 deviceId、 policyId 和用户 Id</span><span class="sxs-lookup"><span data-stu-id="35d6f-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="35d6f-135">userId</span><span class="sxs-lookup"><span data-stu-id="35d6f-135">userId</span></span>|<span data-ttu-id="35d6f-136">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-136">String</span></span>|<span data-ttu-id="35d6f-137">用户的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="35d6f-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="35d6f-138">userName</span><span class="sxs-lookup"><span data-stu-id="35d6f-138">userName</span></span>|<span data-ttu-id="35d6f-139">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-139">String</span></span>|<span data-ttu-id="35d6f-140">用户名</span><span class="sxs-lookup"><span data-stu-id="35d6f-140">User name</span></span>|
|<span data-ttu-id="35d6f-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="35d6f-141">managedDeviceId</span></span>|<span data-ttu-id="35d6f-142">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-142">String</span></span>|<span data-ttu-id="35d6f-143">托管的设备的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="35d6f-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="35d6f-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="35d6f-144">deviceName</span></span>|<span data-ttu-id="35d6f-145">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-145">String</span></span>|<span data-ttu-id="35d6f-146">设备名称</span><span class="sxs-lookup"><span data-stu-id="35d6f-146">Device name</span></span>|
|<span data-ttu-id="35d6f-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="35d6f-147">deviceConfigurationId</span></span>|<span data-ttu-id="35d6f-148">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-148">String</span></span>|<span data-ttu-id="35d6f-149">设备配置配置文件的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="35d6f-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="35d6f-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="35d6f-150">deviceConfigurationName</span></span>|<span data-ttu-id="35d6f-151">String</span><span class="sxs-lookup"><span data-stu-id="35d6f-151">String</span></span>|<span data-ttu-id="35d6f-152">设备配置配置文件名称</span><span class="sxs-lookup"><span data-stu-id="35d6f-152">Device configuration profile name</span></span>|
|<span data-ttu-id="35d6f-153">platformType</span><span class="sxs-lookup"><span data-stu-id="35d6f-153">platformType</span></span>|[<span data-ttu-id="35d6f-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="35d6f-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="35d6f-155">平台类型。</span><span class="sxs-lookup"><span data-stu-id="35d6f-155">Platform type.</span></span> <span data-ttu-id="35d6f-156">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="35d6f-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="35d6f-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="35d6f-157">restrictedAppsState</span></span>|[<span data-ttu-id="35d6f-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="35d6f-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="35d6f-159">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="35d6f-159">Restricted apps state.</span></span> <span data-ttu-id="35d6f-160">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="35d6f-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="35d6f-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="35d6f-161">restrictedApps</span></span>|<span data-ttu-id="35d6f-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d6f-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="35d6f-163">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="35d6f-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d6f-164">关系</span><span class="sxs-lookup"><span data-stu-id="35d6f-164">Relationships</span></span>
<span data-ttu-id="35d6f-165">无</span><span class="sxs-lookup"><span data-stu-id="35d6f-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d6f-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d6f-166">JSON Representation</span></span>
<span data-ttu-id="35d6f-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d6f-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```




