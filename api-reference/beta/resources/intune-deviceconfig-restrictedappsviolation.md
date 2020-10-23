---
title: restrictedAppsViolation 资源类型
description: 每个用户的每个设备违反受限制的应用配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ab38a5dff42bf29dbda301c5dbdb102972716fb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707029"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="36c7f-103">restrictedAppsViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="36c7f-103">restrictedAppsViolation resource type</span></span>

<span data-ttu-id="36c7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36c7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36c7f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36c7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36c7f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36c7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36c7f-107">每个用户的每个设备违反受限制的应用配置文件</span><span class="sxs-lookup"><span data-stu-id="36c7f-107">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="36c7f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="36c7f-108">Methods</span></span>
|<span data-ttu-id="36c7f-109">方法</span><span class="sxs-lookup"><span data-stu-id="36c7f-109">Method</span></span>|<span data-ttu-id="36c7f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="36c7f-110">Return Type</span></span>|<span data-ttu-id="36c7f-111">说明</span><span class="sxs-lookup"><span data-stu-id="36c7f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="36c7f-112">列出 restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="36c7f-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="36c7f-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36c7f-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="36c7f-114">列出 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36c7f-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="36c7f-115">获取 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="36c7f-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="36c7f-117">读取 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36c7f-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="36c7f-118">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="36c7f-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="36c7f-120">创建新的 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36c7f-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="36c7f-121">删除 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="36c7f-122">无</span><span class="sxs-lookup"><span data-stu-id="36c7f-122">None</span></span>|<span data-ttu-id="36c7f-123">删除 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。</span><span class="sxs-lookup"><span data-stu-id="36c7f-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="36c7f-124">更新 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="36c7f-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="36c7f-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="36c7f-126">更新 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="36c7f-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36c7f-127">属性</span><span class="sxs-lookup"><span data-stu-id="36c7f-127">Properties</span></span>
|<span data-ttu-id="36c7f-128">属性</span><span class="sxs-lookup"><span data-stu-id="36c7f-128">Property</span></span>|<span data-ttu-id="36c7f-129">类型</span><span class="sxs-lookup"><span data-stu-id="36c7f-129">Type</span></span>|<span data-ttu-id="36c7f-130">说明</span><span class="sxs-lookup"><span data-stu-id="36c7f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36c7f-131">id</span><span class="sxs-lookup"><span data-stu-id="36c7f-131">id</span></span>|<span data-ttu-id="36c7f-132">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-132">String</span></span>|<span data-ttu-id="36c7f-133">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="36c7f-133">Unique identifier for the object.</span></span> <span data-ttu-id="36c7f-134">由 accountId、deviceId、policyId 和 userId 组成</span><span class="sxs-lookup"><span data-stu-id="36c7f-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="36c7f-135">userId</span><span class="sxs-lookup"><span data-stu-id="36c7f-135">userId</span></span>|<span data-ttu-id="36c7f-136">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-136">String</span></span>|<span data-ttu-id="36c7f-137">用户唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="36c7f-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="36c7f-138">userName</span><span class="sxs-lookup"><span data-stu-id="36c7f-138">userName</span></span>|<span data-ttu-id="36c7f-139">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-139">String</span></span>|<span data-ttu-id="36c7f-140">用户名</span><span class="sxs-lookup"><span data-stu-id="36c7f-140">User name</span></span>|
|<span data-ttu-id="36c7f-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="36c7f-141">managedDeviceId</span></span>|<span data-ttu-id="36c7f-142">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-142">String</span></span>|<span data-ttu-id="36c7f-143">托管设备唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="36c7f-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="36c7f-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="36c7f-144">deviceName</span></span>|<span data-ttu-id="36c7f-145">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-145">String</span></span>|<span data-ttu-id="36c7f-146">设备名称</span><span class="sxs-lookup"><span data-stu-id="36c7f-146">Device name</span></span>|
|<span data-ttu-id="36c7f-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="36c7f-147">deviceConfigurationId</span></span>|<span data-ttu-id="36c7f-148">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-148">String</span></span>|<span data-ttu-id="36c7f-149">设备配置文件唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="36c7f-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="36c7f-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="36c7f-150">deviceConfigurationName</span></span>|<span data-ttu-id="36c7f-151">String</span><span class="sxs-lookup"><span data-stu-id="36c7f-151">String</span></span>|<span data-ttu-id="36c7f-152">设备配置文件名称</span><span class="sxs-lookup"><span data-stu-id="36c7f-152">Device configuration profile name</span></span>|
|<span data-ttu-id="36c7f-153">platformType</span><span class="sxs-lookup"><span data-stu-id="36c7f-153">platformType</span></span>|[<span data-ttu-id="36c7f-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="36c7f-154">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="36c7f-155">平台类型。</span><span class="sxs-lookup"><span data-stu-id="36c7f-155">Platform type.</span></span> <span data-ttu-id="36c7f-156">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="36c7f-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="36c7f-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="36c7f-157">restrictedAppsState</span></span>|[<span data-ttu-id="36c7f-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="36c7f-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="36c7f-159">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="36c7f-159">Restricted apps state.</span></span> <span data-ttu-id="36c7f-160">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="36c7f-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="36c7f-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="36c7f-161">restrictedApps</span></span>|<span data-ttu-id="36c7f-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36c7f-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="36c7f-163">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="36c7f-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="36c7f-164">关系</span><span class="sxs-lookup"><span data-stu-id="36c7f-164">Relationships</span></span>
<span data-ttu-id="36c7f-165">无</span><span class="sxs-lookup"><span data-stu-id="36c7f-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36c7f-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36c7f-166">JSON Representation</span></span>
<span data-ttu-id="36c7f-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36c7f-167">Here is a JSON representation of the resource.</span></span>
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





