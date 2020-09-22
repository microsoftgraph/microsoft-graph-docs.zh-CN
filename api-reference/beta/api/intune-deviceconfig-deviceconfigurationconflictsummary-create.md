---
title: 创建 deviceConfigurationConflictSummary
description: 创建新的 deviceConfigurationConflictSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34071af61f3906b709a3ecf03884ae91569593f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011499"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="18b47-103">创建 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="18b47-103">Create deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="18b47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18b47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18b47-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18b47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18b47-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18b47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b47-107">创建新的 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18b47-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18b47-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="18b47-108">Prerequisites</span></span>
<span data-ttu-id="18b47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18b47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18b47-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18b47-111">Permission type</span></span>|<span data-ttu-id="18b47-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18b47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18b47-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18b47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18b47-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b47-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18b47-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18b47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18b47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18b47-116">Not supported.</span></span>|
|<span data-ttu-id="18b47-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18b47-117">Application</span></span>|<span data-ttu-id="18b47-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b47-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18b47-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18b47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="18b47-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18b47-120">Request headers</span></span>
|<span data-ttu-id="18b47-121">标头</span><span class="sxs-lookup"><span data-stu-id="18b47-121">Header</span></span>|<span data-ttu-id="18b47-122">值</span><span class="sxs-lookup"><span data-stu-id="18b47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18b47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b47-123">Authorization</span></span>|<span data-ttu-id="18b47-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18b47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18b47-125">接受</span><span class="sxs-lookup"><span data-stu-id="18b47-125">Accept</span></span>|<span data-ttu-id="18b47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18b47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18b47-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18b47-127">Request body</span></span>
<span data-ttu-id="18b47-128">在请求正文中，提供 deviceConfigurationConflictSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18b47-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="18b47-129">下表显示创建 deviceConfigurationConflictSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18b47-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="18b47-130">属性</span><span class="sxs-lookup"><span data-stu-id="18b47-130">Property</span></span>|<span data-ttu-id="18b47-131">类型</span><span class="sxs-lookup"><span data-stu-id="18b47-131">Type</span></span>|<span data-ttu-id="18b47-132">说明</span><span class="sxs-lookup"><span data-stu-id="18b47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b47-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="18b47-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="18b47-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="18b47-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="18b47-135">与给定设置发生冲突的策略集</span><span class="sxs-lookup"><span data-stu-id="18b47-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="18b47-136">id</span><span class="sxs-lookup"><span data-stu-id="18b47-136">id</span></span>|<span data-ttu-id="18b47-137">String</span><span class="sxs-lookup"><span data-stu-id="18b47-137">String</span></span>|<span data-ttu-id="18b47-138">此组冲突策略的 id。</span><span class="sxs-lookup"><span data-stu-id="18b47-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="18b47-139">此 id 是 ConflictingDeviceConfigurations 中的所有策略的 id，以字典顺序分隔，由下划线分隔。</span><span class="sxs-lookup"><span data-stu-id="18b47-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="18b47-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="18b47-140">contributingSettings</span></span>|<span data-ttu-id="18b47-141">String collection</span><span class="sxs-lookup"><span data-stu-id="18b47-141">String collection</span></span>|<span data-ttu-id="18b47-142">与给定策略发生冲突的设置集</span><span class="sxs-lookup"><span data-stu-id="18b47-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="18b47-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="18b47-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="18b47-144">Int32</span><span class="sxs-lookup"><span data-stu-id="18b47-144">Int32</span></span>|<span data-ttu-id="18b47-145">受冲突策略和设置影响的签入次数</span><span class="sxs-lookup"><span data-stu-id="18b47-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="18b47-146">响应</span><span class="sxs-lookup"><span data-stu-id="18b47-146">Response</span></span>
<span data-ttu-id="18b47-147">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18b47-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b47-148">示例</span><span class="sxs-lookup"><span data-stu-id="18b47-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="18b47-149">请求</span><span class="sxs-lookup"><span data-stu-id="18b47-149">Request</span></span>
<span data-ttu-id="18b47-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18b47-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 398

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="18b47-151">响应</span><span class="sxs-lookup"><span data-stu-id="18b47-151">Response</span></span>
<span data-ttu-id="18b47-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18b47-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```






