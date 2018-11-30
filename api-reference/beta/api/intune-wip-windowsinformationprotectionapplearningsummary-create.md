---
title: 创建 windowsInformationProtectionAppLearningSummary
description: 创建新的 windowsInformationProtectionAppLearningSummary 对象。
ms.openlocfilehash: 671ab1efd631541871623fd1687639dd3d8d95ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048365"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="12f0f-103">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="12f0f-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="12f0f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12f0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12f0f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12f0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12f0f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12f0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12f0f-107">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12f0f-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12f0f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12f0f-108">Prerequisites</span></span>
<span data-ttu-id="12f0f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="12f0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f0f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12f0f-111">Permission type</span></span>|<span data-ttu-id="12f0f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12f0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12f0f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12f0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12f0f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f0f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12f0f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12f0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12f0f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12f0f-116">Not supported.</span></span>|
|<span data-ttu-id="12f0f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12f0f-117">Application</span></span>|<span data-ttu-id="12f0f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="12f0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12f0f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12f0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="12f0f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12f0f-120">Request headers</span></span>
|<span data-ttu-id="12f0f-121">标头</span><span class="sxs-lookup"><span data-stu-id="12f0f-121">Header</span></span>|<span data-ttu-id="12f0f-122">值</span><span class="sxs-lookup"><span data-stu-id="12f0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12f0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f0f-123">Authorization</span></span>|<span data-ttu-id="12f0f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12f0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12f0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12f0f-125">Accept</span></span>|<span data-ttu-id="12f0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12f0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12f0f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12f0f-127">Request body</span></span>
<span data-ttu-id="12f0f-128">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12f0f-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="12f0f-129">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12f0f-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="12f0f-130">属性</span><span class="sxs-lookup"><span data-stu-id="12f0f-130">Property</span></span>|<span data-ttu-id="12f0f-131">类型</span><span class="sxs-lookup"><span data-stu-id="12f0f-131">Type</span></span>|<span data-ttu-id="12f0f-132">说明</span><span class="sxs-lookup"><span data-stu-id="12f0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f0f-133">id</span><span class="sxs-lookup"><span data-stu-id="12f0f-133">id</span></span>|<span data-ttu-id="12f0f-134">String</span><span class="sxs-lookup"><span data-stu-id="12f0f-134">String</span></span>|<span data-ttu-id="12f0f-135">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12f0f-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="12f0f-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="12f0f-136">applicationName</span></span>|<span data-ttu-id="12f0f-137">String</span><span class="sxs-lookup"><span data-stu-id="12f0f-137">String</span></span>|<span data-ttu-id="12f0f-138">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="12f0f-138">Application Name</span></span>|
|<span data-ttu-id="12f0f-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="12f0f-139">applicationType</span></span>|[<span data-ttu-id="12f0f-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="12f0f-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="12f0f-141">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="12f0f-141">Application Type.</span></span> <span data-ttu-id="12f0f-142">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="12f0f-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="12f0f-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="12f0f-143">deviceCount</span></span>|<span data-ttu-id="12f0f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="12f0f-144">Int32</span></span>|<span data-ttu-id="12f0f-145">设备计数</span><span class="sxs-lookup"><span data-stu-id="12f0f-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="12f0f-146">响应</span><span class="sxs-lookup"><span data-stu-id="12f0f-146">Response</span></span>
<span data-ttu-id="12f0f-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12f0f-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f0f-148">示例</span><span class="sxs-lookup"><span data-stu-id="12f0f-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="12f0f-149">请求</span><span class="sxs-lookup"><span data-stu-id="12f0f-149">Request</span></span>
<span data-ttu-id="12f0f-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12f0f-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="12f0f-151">响应</span><span class="sxs-lookup"><span data-stu-id="12f0f-151">Response</span></span>
<span data-ttu-id="12f0f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12f0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```





