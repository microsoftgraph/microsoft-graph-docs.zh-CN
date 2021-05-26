---
title: restrictedAppsViolation 资源类型
description: 每个用户的设备违反受限制的应用配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a328938975b67ebce005f3cee05fb753f051ad49
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665509"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="f943a-103">restrictedAppsViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f943a-103">restrictedAppsViolation resource type</span></span>

<span data-ttu-id="f943a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f943a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f943a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f943a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f943a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f943a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f943a-107">每个用户的设备违反受限制的应用配置文件</span><span class="sxs-lookup"><span data-stu-id="f943a-107">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="f943a-108">方法</span><span class="sxs-lookup"><span data-stu-id="f943a-108">Methods</span></span>
|<span data-ttu-id="f943a-109">方法</span><span class="sxs-lookup"><span data-stu-id="f943a-109">Method</span></span>|<span data-ttu-id="f943a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f943a-110">Return Type</span></span>|<span data-ttu-id="f943a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f943a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f943a-112">列出 restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="f943a-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="f943a-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f943a-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="f943a-114">列出 [restrictedAppsViolation 对象的属性和](../resources/intune-deviceconfig-restrictedappsviolation.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="f943a-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="f943a-115">获取 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="f943a-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="f943a-117">读取 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f943a-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="f943a-118">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="f943a-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="f943a-120">创建新的 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f943a-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="f943a-121">删除 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="f943a-122">无</span><span class="sxs-lookup"><span data-stu-id="f943a-122">None</span></span>|<span data-ttu-id="f943a-123">删除 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。</span><span class="sxs-lookup"><span data-stu-id="f943a-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="f943a-124">更新 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="f943a-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f943a-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="f943a-126">更新 [restrictedAppsViolation 对象](../resources/intune-deviceconfig-restrictedappsviolation.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f943a-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f943a-127">属性</span><span class="sxs-lookup"><span data-stu-id="f943a-127">Properties</span></span>
|<span data-ttu-id="f943a-128">属性</span><span class="sxs-lookup"><span data-stu-id="f943a-128">Property</span></span>|<span data-ttu-id="f943a-129">类型</span><span class="sxs-lookup"><span data-stu-id="f943a-129">Type</span></span>|<span data-ttu-id="f943a-130">说明</span><span class="sxs-lookup"><span data-stu-id="f943a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f943a-131">id</span><span class="sxs-lookup"><span data-stu-id="f943a-131">id</span></span>|<span data-ttu-id="f943a-132">String</span><span class="sxs-lookup"><span data-stu-id="f943a-132">String</span></span>|<span data-ttu-id="f943a-133">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f943a-133">Unique identifier for the object.</span></span> <span data-ttu-id="f943a-134">由 accountId、deviceId、policyId 和 userId 组成</span><span class="sxs-lookup"><span data-stu-id="f943a-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="f943a-135">userId</span><span class="sxs-lookup"><span data-stu-id="f943a-135">userId</span></span>|<span data-ttu-id="f943a-136">String</span><span class="sxs-lookup"><span data-stu-id="f943a-136">String</span></span>|<span data-ttu-id="f943a-137">用户唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="f943a-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="f943a-138">userName</span><span class="sxs-lookup"><span data-stu-id="f943a-138">userName</span></span>|<span data-ttu-id="f943a-139">String</span><span class="sxs-lookup"><span data-stu-id="f943a-139">String</span></span>|<span data-ttu-id="f943a-140">用户名</span><span class="sxs-lookup"><span data-stu-id="f943a-140">User name</span></span>|
|<span data-ttu-id="f943a-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f943a-141">managedDeviceId</span></span>|<span data-ttu-id="f943a-142">String</span><span class="sxs-lookup"><span data-stu-id="f943a-142">String</span></span>|<span data-ttu-id="f943a-143">托管设备唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="f943a-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="f943a-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="f943a-144">deviceName</span></span>|<span data-ttu-id="f943a-145">String</span><span class="sxs-lookup"><span data-stu-id="f943a-145">String</span></span>|<span data-ttu-id="f943a-146">设备名称</span><span class="sxs-lookup"><span data-stu-id="f943a-146">Device name</span></span>|
|<span data-ttu-id="f943a-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f943a-147">deviceConfigurationId</span></span>|<span data-ttu-id="f943a-148">String</span><span class="sxs-lookup"><span data-stu-id="f943a-148">String</span></span>|<span data-ttu-id="f943a-149">设备配置文件的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="f943a-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="f943a-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="f943a-150">deviceConfigurationName</span></span>|<span data-ttu-id="f943a-151">String</span><span class="sxs-lookup"><span data-stu-id="f943a-151">String</span></span>|<span data-ttu-id="f943a-152">设备配置文件名称</span><span class="sxs-lookup"><span data-stu-id="f943a-152">Device configuration profile name</span></span>|
|<span data-ttu-id="f943a-153">platformType</span><span class="sxs-lookup"><span data-stu-id="f943a-153">platformType</span></span>|[<span data-ttu-id="f943a-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="f943a-154">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="f943a-155">平台类型。</span><span class="sxs-lookup"><span data-stu-id="f943a-155">Platform type.</span></span> <span data-ttu-id="f943a-156">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`androidAOSP`、`all`。</span><span class="sxs-lookup"><span data-stu-id="f943a-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `androidAOSP`, `all`.</span></span>|
|<span data-ttu-id="f943a-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="f943a-157">restrictedAppsState</span></span>|[<span data-ttu-id="f943a-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="f943a-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="f943a-159">受限制的应用状态。</span><span class="sxs-lookup"><span data-stu-id="f943a-159">Restricted apps state.</span></span> <span data-ttu-id="f943a-160">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="f943a-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="f943a-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="f943a-161">restrictedApps</span></span>|<span data-ttu-id="f943a-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f943a-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="f943a-163">违反的受限应用列表</span><span class="sxs-lookup"><span data-stu-id="f943a-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="f943a-164">关系</span><span class="sxs-lookup"><span data-stu-id="f943a-164">Relationships</span></span>
<span data-ttu-id="f943a-165">无</span><span class="sxs-lookup"><span data-stu-id="f943a-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f943a-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f943a-166">JSON Representation</span></span>
<span data-ttu-id="f943a-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f943a-167">Here is a JSON representation of the resource.</span></span>
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




