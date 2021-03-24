---
title: 更新 deviceConfigurationConflictSummary
description: 更新 deviceConfigurationConflictSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec2a44fcba9728b0866c4ac1366a46473c443ec5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131692"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="39f05-103">更新 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="39f05-103">Update deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="39f05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39f05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39f05-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="39f05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39f05-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39f05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39f05-107">更新 [deviceConfigurationConflictSummary 对象](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="39f05-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39f05-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="39f05-108">Prerequisites</span></span>
<span data-ttu-id="39f05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39f05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f05-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39f05-111">Permission type</span></span>|<span data-ttu-id="39f05-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39f05-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39f05-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39f05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39f05-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f05-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39f05-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39f05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39f05-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="39f05-116">Not supported.</span></span>|
|<span data-ttu-id="39f05-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39f05-117">Application</span></span>|<span data-ttu-id="39f05-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f05-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39f05-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39f05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="39f05-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="39f05-120">Request headers</span></span>
|<span data-ttu-id="39f05-121">标头</span><span class="sxs-lookup"><span data-stu-id="39f05-121">Header</span></span>|<span data-ttu-id="39f05-122">值</span><span class="sxs-lookup"><span data-stu-id="39f05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39f05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39f05-123">Authorization</span></span>|<span data-ttu-id="39f05-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39f05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39f05-125">接受</span><span class="sxs-lookup"><span data-stu-id="39f05-125">Accept</span></span>|<span data-ttu-id="39f05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39f05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39f05-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39f05-127">Request body</span></span>
<span data-ttu-id="39f05-128">在请求正文中，提供 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39f05-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="39f05-129">下表显示创建 [deviceConfigurationConflictSummary 时所需的属性](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="39f05-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="39f05-130">属性</span><span class="sxs-lookup"><span data-stu-id="39f05-130">Property</span></span>|<span data-ttu-id="39f05-131">类型</span><span class="sxs-lookup"><span data-stu-id="39f05-131">Type</span></span>|<span data-ttu-id="39f05-132">说明</span><span class="sxs-lookup"><span data-stu-id="39f05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f05-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="39f05-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="39f05-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39f05-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="39f05-135">与给定设置相冲突的策略集</span><span class="sxs-lookup"><span data-stu-id="39f05-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="39f05-136">id</span><span class="sxs-lookup"><span data-stu-id="39f05-136">id</span></span>|<span data-ttu-id="39f05-137">String</span><span class="sxs-lookup"><span data-stu-id="39f05-137">String</span></span>|<span data-ttu-id="39f05-138">这组冲突策略的 ID。</span><span class="sxs-lookup"><span data-stu-id="39f05-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="39f05-139">此 id 是 ConflictingDeviceConfigurations 中所有策略的 ID，按字典顺序使用下划线分隔。</span><span class="sxs-lookup"><span data-stu-id="39f05-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="39f05-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="39f05-140">contributingSettings</span></span>|<span data-ttu-id="39f05-141">String collection</span><span class="sxs-lookup"><span data-stu-id="39f05-141">String collection</span></span>|<span data-ttu-id="39f05-142">与给定策略相冲突的设置集</span><span class="sxs-lookup"><span data-stu-id="39f05-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="39f05-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="39f05-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="39f05-144">Int32</span><span class="sxs-lookup"><span data-stu-id="39f05-144">Int32</span></span>|<span data-ttu-id="39f05-145">受冲突策略和设置影响的签入计数</span><span class="sxs-lookup"><span data-stu-id="39f05-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="39f05-146">响应</span><span class="sxs-lookup"><span data-stu-id="39f05-146">Response</span></span>
<span data-ttu-id="39f05-147">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39f05-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39f05-148">示例</span><span class="sxs-lookup"><span data-stu-id="39f05-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="39f05-149">请求</span><span class="sxs-lookup"><span data-stu-id="39f05-149">Request</span></span>
<span data-ttu-id="39f05-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39f05-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
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

### <a name="response"></a><span data-ttu-id="39f05-151">响应</span><span class="sxs-lookup"><span data-stu-id="39f05-151">Response</span></span>
<span data-ttu-id="39f05-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39f05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




