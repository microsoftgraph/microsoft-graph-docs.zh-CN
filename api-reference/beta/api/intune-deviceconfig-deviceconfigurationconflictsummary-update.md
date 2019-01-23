---
title: 更新 deviceConfigurationConflictSummary
description: 更新 deviceConfigurationConflictSummary 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ad5c5c7ad9db02afed53b4deb0cb6af3d2c57e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416354"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="aa6f5-103">更新 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="aa6f5-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="aa6f5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa6f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa6f5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa6f5-107">更新[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa6f5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa6f5-108">Prerequisites</span></span>
<span data-ttu-id="aa6f5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aa6f5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa6f5-111">Permission type</span></span>|<span data-ttu-id="aa6f5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa6f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa6f5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa6f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa6f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa6f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa6f5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa6f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa6f5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-116">Not supported.</span></span>|
|<span data-ttu-id="aa6f5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa6f5-117">Application</span></span>|<span data-ttu-id="aa6f5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa6f5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa6f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="aa6f5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa6f5-120">Request headers</span></span>
|<span data-ttu-id="aa6f5-121">标头</span><span class="sxs-lookup"><span data-stu-id="aa6f5-121">Header</span></span>|<span data-ttu-id="aa6f5-122">值</span><span class="sxs-lookup"><span data-stu-id="aa6f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa6f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa6f5-123">Authorization</span></span>|<span data-ttu-id="aa6f5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa6f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa6f5-125">Accept</span></span>|<span data-ttu-id="aa6f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa6f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa6f5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa6f5-127">Request body</span></span>
<span data-ttu-id="aa6f5-128">在请求正文中，提供[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="aa6f5-129">下表显示时创建[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="aa6f5-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa6f5-130">Property</span></span>|<span data-ttu-id="aa6f5-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa6f5-131">Type</span></span>|<span data-ttu-id="aa6f5-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa6f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa6f5-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="aa6f5-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="aa6f5-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa6f5-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="aa6f5-135">组策略的给定设置冲突</span><span class="sxs-lookup"><span data-stu-id="aa6f5-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="aa6f5-136">id</span><span class="sxs-lookup"><span data-stu-id="aa6f5-136">id</span></span>|<span data-ttu-id="aa6f5-137">String</span><span class="sxs-lookup"><span data-stu-id="aa6f5-137">String</span></span>|<span data-ttu-id="aa6f5-138">冲突策略的这组 id。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="aa6f5-139">此 id 是分隔下划线字典顺序 ConflictingDeviceConfigurations 中的所有策略的 id。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="aa6f5-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="aa6f5-140">contributingSettings</span></span>|<span data-ttu-id="aa6f5-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="aa6f5-141">String collection</span></span>|<span data-ttu-id="aa6f5-142">冲突的给定的策略设置的集合</span><span class="sxs-lookup"><span data-stu-id="aa6f5-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="aa6f5-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="aa6f5-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="aa6f5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="aa6f5-144">Int32</span></span>|<span data-ttu-id="aa6f5-145">签入受影响的冲突的策略和设置的计数</span><span class="sxs-lookup"><span data-stu-id="aa6f5-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="aa6f5-146">响应</span><span class="sxs-lookup"><span data-stu-id="aa6f5-146">Response</span></span>
<span data-ttu-id="aa6f5-147">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa6f5-148">示例</span><span class="sxs-lookup"><span data-stu-id="aa6f5-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa6f5-149">请求</span><span class="sxs-lookup"><span data-stu-id="aa6f5-149">Request</span></span>
<span data-ttu-id="aa6f5-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
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

### <a name="response"></a><span data-ttu-id="aa6f5-151">响应</span><span class="sxs-lookup"><span data-stu-id="aa6f5-151">Response</span></span>
<span data-ttu-id="aa6f5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




