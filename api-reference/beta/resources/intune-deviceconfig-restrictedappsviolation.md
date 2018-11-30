---
title: restrictedAppsViolation 资源类型
description: 与每个每个用户的设备的受限的应用程序配置文件的冲突
ms.openlocfilehash: 6d7f6cb8b52671c311c39c3306a329ad37194b85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047679"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="8a96a-103">restrictedAppsViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a96a-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="8a96a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8a96a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a96a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8a96a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a96a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8a96a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a96a-107">与每个每个用户的设备的受限的应用程序配置文件的冲突</span><span class="sxs-lookup"><span data-stu-id="8a96a-107">Violation of restricted apps configuration profile per device per user</span></span>
## <a name="methods"></a><span data-ttu-id="8a96a-108">方法</span><span class="sxs-lookup"><span data-stu-id="8a96a-108">Methods</span></span>
|<span data-ttu-id="8a96a-109">方法</span><span class="sxs-lookup"><span data-stu-id="8a96a-109">Method</span></span>|<span data-ttu-id="8a96a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a96a-110">Return Type</span></span>|<span data-ttu-id="8a96a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8a96a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a96a-112">列表 restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="8a96a-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="8a96a-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a96a-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="8a96a-114">列出属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="8a96a-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="8a96a-115">获取 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="8a96a-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="8a96a-117">读取属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="8a96a-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="8a96a-118">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="8a96a-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="8a96a-120">创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8a96a-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="8a96a-121">删除 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="8a96a-122">无</span><span class="sxs-lookup"><span data-stu-id="8a96a-122">None</span></span>|<span data-ttu-id="8a96a-123">删除[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。</span><span class="sxs-lookup"><span data-stu-id="8a96a-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="8a96a-124">更新 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="8a96a-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="8a96a-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="8a96a-126">更新[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8a96a-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a96a-127">属性</span><span class="sxs-lookup"><span data-stu-id="8a96a-127">Properties</span></span>
|<span data-ttu-id="8a96a-128">属性</span><span class="sxs-lookup"><span data-stu-id="8a96a-128">Property</span></span>|<span data-ttu-id="8a96a-129">类型</span><span class="sxs-lookup"><span data-stu-id="8a96a-129">Type</span></span>|<span data-ttu-id="8a96a-130">说明</span><span class="sxs-lookup"><span data-stu-id="8a96a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a96a-131">id</span><span class="sxs-lookup"><span data-stu-id="8a96a-131">id</span></span>|<span data-ttu-id="8a96a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="8a96a-132">String</span></span>|<span data-ttu-id="8a96a-133">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a96a-133">Unique identifier for the object.</span></span> <span data-ttu-id="8a96a-134">由 accountId、 deviceId、 policyId 和用户 Id</span><span class="sxs-lookup"><span data-stu-id="8a96a-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="8a96a-135">userId</span><span class="sxs-lookup"><span data-stu-id="8a96a-135">userId</span></span>|<span data-ttu-id="8a96a-136">String</span><span class="sxs-lookup"><span data-stu-id="8a96a-136">String</span></span>|<span data-ttu-id="8a96a-137">用户的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="8a96a-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="8a96a-138">userName</span><span class="sxs-lookup"><span data-stu-id="8a96a-138">userName</span></span>|<span data-ttu-id="8a96a-139">String</span><span class="sxs-lookup"><span data-stu-id="8a96a-139">String</span></span>|<span data-ttu-id="8a96a-140">用户名</span><span class="sxs-lookup"><span data-stu-id="8a96a-140">User name</span></span>|
|<span data-ttu-id="8a96a-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8a96a-141">managedDeviceId</span></span>|<span data-ttu-id="8a96a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="8a96a-142">String</span></span>|<span data-ttu-id="8a96a-143">托管的设备的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="8a96a-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="8a96a-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="8a96a-144">deviceName</span></span>|<span data-ttu-id="8a96a-145">String</span><span class="sxs-lookup"><span data-stu-id="8a96a-145">String</span></span>|<span data-ttu-id="8a96a-146">设备名称</span><span class="sxs-lookup"><span data-stu-id="8a96a-146">Device name</span></span>|
|<span data-ttu-id="8a96a-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8a96a-147">deviceConfigurationId</span></span>|<span data-ttu-id="8a96a-148">字符串</span><span class="sxs-lookup"><span data-stu-id="8a96a-148">String</span></span>|<span data-ttu-id="8a96a-149">设备配置配置文件的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="8a96a-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="8a96a-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="8a96a-150">deviceConfigurationName</span></span>|<span data-ttu-id="8a96a-151">字符串</span><span class="sxs-lookup"><span data-stu-id="8a96a-151">String</span></span>|<span data-ttu-id="8a96a-152">设备配置配置文件名称</span><span class="sxs-lookup"><span data-stu-id="8a96a-152">Device configuration profile name</span></span>|
|<span data-ttu-id="8a96a-153">platformType</span><span class="sxs-lookup"><span data-stu-id="8a96a-153">platformType</span></span>|[<span data-ttu-id="8a96a-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="8a96a-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="8a96a-155">平台类型。</span><span class="sxs-lookup"><span data-stu-id="8a96a-155">Platform type.</span></span> <span data-ttu-id="8a96a-156">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="8a96a-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="8a96a-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="8a96a-157">restrictedAppsState</span></span>|[<span data-ttu-id="8a96a-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="8a96a-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="8a96a-159">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="8a96a-159">Restricted apps state.</span></span> <span data-ttu-id="8a96a-160">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="8a96a-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="8a96a-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="8a96a-161">restrictedApps</span></span>|<span data-ttu-id="8a96a-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a96a-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="8a96a-163">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="8a96a-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a96a-164">Relationships</span><span class="sxs-lookup"><span data-stu-id="8a96a-164">Relationships</span></span>
<span data-ttu-id="8a96a-165">无</span><span class="sxs-lookup"><span data-stu-id="8a96a-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a96a-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a96a-166">JSON Representation</span></span>
<span data-ttu-id="8a96a-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a96a-167">Here is a JSON representation of the resource.</span></span>
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





