---
title: 创建 deviceConfigurationConflictSummary
description: 创建新的 deviceConfigurationConflictSummary 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a027083cac6ef997c69c8bb1b3d4e8d85237fd7b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168305"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="75daf-103">创建 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="75daf-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="75daf-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75daf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75daf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75daf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75daf-106">创建新的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="75daf-106">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75daf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="75daf-107">Prerequisites</span></span>
<span data-ttu-id="75daf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75daf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75daf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75daf-110">Permission type</span></span>|<span data-ttu-id="75daf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="75daf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75daf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75daf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75daf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75daf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75daf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75daf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75daf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75daf-115">Not supported.</span></span>|
|<span data-ttu-id="75daf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="75daf-116">Application</span></span>|<span data-ttu-id="75daf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75daf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75daf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75daf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="75daf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75daf-119">Request headers</span></span>
|<span data-ttu-id="75daf-120">标头</span><span class="sxs-lookup"><span data-stu-id="75daf-120">Header</span></span>|<span data-ttu-id="75daf-121">值</span><span class="sxs-lookup"><span data-stu-id="75daf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75daf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75daf-122">Authorization</span></span>|<span data-ttu-id="75daf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="75daf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75daf-124">接受</span><span class="sxs-lookup"><span data-stu-id="75daf-124">Accept</span></span>|<span data-ttu-id="75daf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75daf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75daf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="75daf-126">Request body</span></span>
<span data-ttu-id="75daf-127">在请求正文中，提供 deviceConfigurationConflictSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75daf-127">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="75daf-128">下表显示创建 deviceConfigurationConflictSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="75daf-128">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="75daf-129">属性</span><span class="sxs-lookup"><span data-stu-id="75daf-129">Property</span></span>|<span data-ttu-id="75daf-130">类型</span><span class="sxs-lookup"><span data-stu-id="75daf-130">Type</span></span>|<span data-ttu-id="75daf-131">说明</span><span class="sxs-lookup"><span data-stu-id="75daf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75daf-132">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="75daf-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="75daf-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75daf-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="75daf-134">与给定设置发生冲突的策略集</span><span class="sxs-lookup"><span data-stu-id="75daf-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="75daf-135">id</span><span class="sxs-lookup"><span data-stu-id="75daf-135">id</span></span>|<span data-ttu-id="75daf-136">String</span><span class="sxs-lookup"><span data-stu-id="75daf-136">String</span></span>|<span data-ttu-id="75daf-137">此组冲突策略的 id。</span><span class="sxs-lookup"><span data-stu-id="75daf-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="75daf-138">此 id 是 ConflictingDeviceConfigurations 中的所有策略的 id，以字典顺序分隔，由下划线分隔。</span><span class="sxs-lookup"><span data-stu-id="75daf-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="75daf-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="75daf-139">contributingSettings</span></span>|<span data-ttu-id="75daf-140">String collection</span><span class="sxs-lookup"><span data-stu-id="75daf-140">String collection</span></span>|<span data-ttu-id="75daf-141">与给定策略发生冲突的设置集</span><span class="sxs-lookup"><span data-stu-id="75daf-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="75daf-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="75daf-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="75daf-143">Int32</span><span class="sxs-lookup"><span data-stu-id="75daf-143">Int32</span></span>|<span data-ttu-id="75daf-144">受冲突策略和设置影响的签入次数</span><span class="sxs-lookup"><span data-stu-id="75daf-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="75daf-145">响应</span><span class="sxs-lookup"><span data-stu-id="75daf-145">Response</span></span>
<span data-ttu-id="75daf-146">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="75daf-146">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75daf-147">示例</span><span class="sxs-lookup"><span data-stu-id="75daf-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="75daf-148">请求</span><span class="sxs-lookup"><span data-stu-id="75daf-148">Request</span></span>
<span data-ttu-id="75daf-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75daf-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="75daf-150">响应</span><span class="sxs-lookup"><span data-stu-id="75daf-150">Response</span></span>
<span data-ttu-id="75daf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75daf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




