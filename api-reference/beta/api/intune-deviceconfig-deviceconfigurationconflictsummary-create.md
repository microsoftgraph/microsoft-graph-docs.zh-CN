---
title: 创建 deviceConfigurationConflictSummary
description: 创建新的 deviceConfigurationConflictSummary 对象。
ms.openlocfilehash: 05532150c01c49e832e28ac811f68afcc00da651
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041253"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="2e535-103">创建 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="2e535-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="2e535-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2e535-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e535-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2e535-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e535-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2e535-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e535-107">创建新的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2e535-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e535-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e535-108">Prerequisites</span></span>
<span data-ttu-id="2e535-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2e535-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e535-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e535-111">Permission type</span></span>|<span data-ttu-id="2e535-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e535-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e535-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e535-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e535-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e535-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e535-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e535-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e535-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e535-116">Not supported.</span></span>|
|<span data-ttu-id="2e535-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e535-117">Application</span></span>|<span data-ttu-id="2e535-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e535-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e535-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e535-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="2e535-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e535-120">Request headers</span></span>
|<span data-ttu-id="2e535-121">标头</span><span class="sxs-lookup"><span data-stu-id="2e535-121">Header</span></span>|<span data-ttu-id="2e535-122">值</span><span class="sxs-lookup"><span data-stu-id="2e535-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e535-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e535-123">Authorization</span></span>|<span data-ttu-id="2e535-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e535-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e535-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e535-125">Accept</span></span>|<span data-ttu-id="2e535-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e535-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e535-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e535-127">Request body</span></span>
<span data-ttu-id="2e535-128">在请求正文中，提供 deviceConfigurationConflictSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e535-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="2e535-129">下表显示时创建 deviceConfigurationConflictSummary 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e535-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="2e535-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e535-130">Property</span></span>|<span data-ttu-id="2e535-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e535-131">Type</span></span>|<span data-ttu-id="2e535-132">说明</span><span class="sxs-lookup"><span data-stu-id="2e535-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e535-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="2e535-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="2e535-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e535-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="2e535-135">组策略的给定设置冲突</span><span class="sxs-lookup"><span data-stu-id="2e535-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="2e535-136">id</span><span class="sxs-lookup"><span data-stu-id="2e535-136">id</span></span>|<span data-ttu-id="2e535-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2e535-137">String</span></span>|<span data-ttu-id="2e535-138">冲突策略的这组 id。</span><span class="sxs-lookup"><span data-stu-id="2e535-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="2e535-139">此 id 是分隔下划线字典顺序 ConflictingDeviceConfigurations 中的所有策略的 id。</span><span class="sxs-lookup"><span data-stu-id="2e535-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="2e535-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="2e535-140">contributingSettings</span></span>|<span data-ttu-id="2e535-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="2e535-141">String collection</span></span>|<span data-ttu-id="2e535-142">冲突的给定的策略设置的集合</span><span class="sxs-lookup"><span data-stu-id="2e535-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="2e535-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="2e535-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="2e535-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2e535-144">Int32</span></span>|<span data-ttu-id="2e535-145">签入受影响的冲突的策略和设置的计数</span><span class="sxs-lookup"><span data-stu-id="2e535-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="2e535-146">响应</span><span class="sxs-lookup"><span data-stu-id="2e535-146">Response</span></span>
<span data-ttu-id="2e535-147">如果成功，此方法返回`201 Created`响应代码和响应正文中的[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2e535-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e535-148">示例</span><span class="sxs-lookup"><span data-stu-id="2e535-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e535-149">请求</span><span class="sxs-lookup"><span data-stu-id="2e535-149">Request</span></span>
<span data-ttu-id="2e535-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e535-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e535-151">响应</span><span class="sxs-lookup"><span data-stu-id="2e535-151">Response</span></span>
<span data-ttu-id="2e535-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e535-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





