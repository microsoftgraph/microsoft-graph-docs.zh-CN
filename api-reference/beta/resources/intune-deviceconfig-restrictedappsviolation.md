---
title: restrictedAppsViolation 资源类型
description: 每个用户的每个设备违反受限制的应用配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8764d3d84ba0706f3769ef019def43cb080660d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139912"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="b3ba7-103">restrictedAppsViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3ba7-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="b3ba7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ba7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ba7-106">每个用户的每个设备违反受限制的应用配置文件</span><span class="sxs-lookup"><span data-stu-id="b3ba7-106">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="b3ba7-107">方法</span><span class="sxs-lookup"><span data-stu-id="b3ba7-107">Methods</span></span>
|<span data-ttu-id="b3ba7-108">方法</span><span class="sxs-lookup"><span data-stu-id="b3ba7-108">Method</span></span>|<span data-ttu-id="b3ba7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3ba7-109">Return Type</span></span>|<span data-ttu-id="b3ba7-110">说明</span><span class="sxs-lookup"><span data-stu-id="b3ba7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3ba7-111">列出 restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="b3ba7-111">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="b3ba7-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3ba7-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="b3ba7-113">列出[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-113">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="b3ba7-114">获取 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-114">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="b3ba7-115">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-115">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="b3ba7-116">读取[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-116">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="b3ba7-117">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-117">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="b3ba7-118">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-118">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="b3ba7-119">创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-119">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="b3ba7-120">删除 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-120">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="b3ba7-121">无</span><span class="sxs-lookup"><span data-stu-id="b3ba7-121">None</span></span>|<span data-ttu-id="b3ba7-122">删除[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-122">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="b3ba7-123">更新 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-123">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="b3ba7-124">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="b3ba7-124">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="b3ba7-125">更新[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-125">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3ba7-126">属性</span><span class="sxs-lookup"><span data-stu-id="b3ba7-126">Properties</span></span>
|<span data-ttu-id="b3ba7-127">属性</span><span class="sxs-lookup"><span data-stu-id="b3ba7-127">Property</span></span>|<span data-ttu-id="b3ba7-128">类型</span><span class="sxs-lookup"><span data-stu-id="b3ba7-128">Type</span></span>|<span data-ttu-id="b3ba7-129">说明</span><span class="sxs-lookup"><span data-stu-id="b3ba7-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3ba7-130">id</span><span class="sxs-lookup"><span data-stu-id="b3ba7-130">id</span></span>|<span data-ttu-id="b3ba7-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ba7-131">String</span></span>|<span data-ttu-id="b3ba7-132">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-132">Unique identifier for the object.</span></span> <span data-ttu-id="b3ba7-133">由 accountId、deviceId、policyId 和 userId 组成</span><span class="sxs-lookup"><span data-stu-id="b3ba7-133">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="b3ba7-134">userId</span><span class="sxs-lookup"><span data-stu-id="b3ba7-134">userId</span></span>|<span data-ttu-id="b3ba7-135">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ba7-135">String</span></span>|<span data-ttu-id="b3ba7-136">用户唯一标识符, 必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="b3ba7-136">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="b3ba7-137">userName</span><span class="sxs-lookup"><span data-stu-id="b3ba7-137">userName</span></span>|<span data-ttu-id="b3ba7-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ba7-138">String</span></span>|<span data-ttu-id="b3ba7-139">用户名</span><span class="sxs-lookup"><span data-stu-id="b3ba7-139">User name</span></span>|
|<span data-ttu-id="b3ba7-140">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b3ba7-140">managedDeviceId</span></span>|<span data-ttu-id="b3ba7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ba7-141">String</span></span>|<span data-ttu-id="b3ba7-142">托管设备唯一标识符, 必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="b3ba7-142">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="b3ba7-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="b3ba7-143">deviceName</span></span>|<span data-ttu-id="b3ba7-144">String</span><span class="sxs-lookup"><span data-stu-id="b3ba7-144">String</span></span>|<span data-ttu-id="b3ba7-145">设备名称</span><span class="sxs-lookup"><span data-stu-id="b3ba7-145">Device name</span></span>|
|<span data-ttu-id="b3ba7-146">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b3ba7-146">deviceConfigurationId</span></span>|<span data-ttu-id="b3ba7-147">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ba7-147">String</span></span>|<span data-ttu-id="b3ba7-148">设备配置文件唯一标识符, 必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="b3ba7-148">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="b3ba7-149">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="b3ba7-149">deviceConfigurationName</span></span>|<span data-ttu-id="b3ba7-150">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ba7-150">String</span></span>|<span data-ttu-id="b3ba7-151">设备配置文件名称</span><span class="sxs-lookup"><span data-stu-id="b3ba7-151">Device configuration profile name</span></span>|
|<span data-ttu-id="b3ba7-152">platformType</span><span class="sxs-lookup"><span data-stu-id="b3ba7-152">platformType</span></span>|[<span data-ttu-id="b3ba7-153">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="b3ba7-153">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="b3ba7-154">平台类型。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-154">Platform type.</span></span> <span data-ttu-id="b3ba7-155">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="b3ba7-156">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="b3ba7-156">restrictedAppsState</span></span>|[<span data-ttu-id="b3ba7-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="b3ba7-157">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="b3ba7-158">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-158">Restricted apps state.</span></span> <span data-ttu-id="b3ba7-159">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-159">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="b3ba7-160">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="b3ba7-160">restrictedApps</span></span>|<span data-ttu-id="b3ba7-161">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3ba7-161">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="b3ba7-162">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="b3ba7-162">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3ba7-163">关系</span><span class="sxs-lookup"><span data-stu-id="b3ba7-163">Relationships</span></span>
<span data-ttu-id="b3ba7-164">无</span><span class="sxs-lookup"><span data-stu-id="b3ba7-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3ba7-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3ba7-165">JSON Representation</span></span>
<span data-ttu-id="b3ba7-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3ba7-166">Here is a JSON representation of the resource.</span></span>
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




