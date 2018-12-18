---
title: 更新 windowsInformationProtectionAppLearningSummary
description: 更新 windowsInformationProtectionAppLearningSummary 对象的属性。
author: tfitzmac
ms.openlocfilehash: 92302f282987a4cc6c56fbf3347e419696f58ee4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354318"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="1ebd8-103">更新 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="1ebd8-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="1ebd8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ebd8-105">更新 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ebd8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ebd8-106">Prerequisites</span></span>
<span data-ttu-id="1ebd8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1ebd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ebd8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ebd8-109">Permission type</span></span>|<span data-ttu-id="1ebd8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ebd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ebd8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ebd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ebd8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ebd8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ebd8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ebd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ebd8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-114">Not supported.</span></span>|
|<span data-ttu-id="1ebd8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ebd8-115">Application</span></span>|<span data-ttu-id="1ebd8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ebd8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ebd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1ebd8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ebd8-118">Request headers</span></span>
|<span data-ttu-id="1ebd8-119">标头</span><span class="sxs-lookup"><span data-stu-id="1ebd8-119">Header</span></span>|<span data-ttu-id="1ebd8-120">值</span><span class="sxs-lookup"><span data-stu-id="1ebd8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ebd8-121">授权</span><span class="sxs-lookup"><span data-stu-id="1ebd8-121">Authorization</span></span>|<span data-ttu-id="1ebd8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ebd8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1ebd8-123">Accept</span></span>|<span data-ttu-id="1ebd8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ebd8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ebd8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ebd8-125">Request body</span></span>
<span data-ttu-id="1ebd8-126">在请求正文中，提供 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="1ebd8-127">下表显示创建 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="1ebd8-128">属性</span><span class="sxs-lookup"><span data-stu-id="1ebd8-128">Property</span></span>|<span data-ttu-id="1ebd8-129">类型</span><span class="sxs-lookup"><span data-stu-id="1ebd8-129">Type</span></span>|<span data-ttu-id="1ebd8-130">说明</span><span class="sxs-lookup"><span data-stu-id="1ebd8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ebd8-131">id</span><span class="sxs-lookup"><span data-stu-id="1ebd8-131">id</span></span>|<span data-ttu-id="1ebd8-132">String</span><span class="sxs-lookup"><span data-stu-id="1ebd8-132">String</span></span>|<span data-ttu-id="1ebd8-133">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="1ebd8-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="1ebd8-134">applicationName</span></span>|<span data-ttu-id="1ebd8-135">String</span><span class="sxs-lookup"><span data-stu-id="1ebd8-135">String</span></span>|<span data-ttu-id="1ebd8-136">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="1ebd8-136">Application Name</span></span>|
|<span data-ttu-id="1ebd8-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="1ebd8-137">applicationType</span></span>|[<span data-ttu-id="1ebd8-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="1ebd8-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="1ebd8-139">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-139">Application Type.</span></span> <span data-ttu-id="1ebd8-140">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="1ebd8-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1ebd8-141">deviceCount</span></span>|<span data-ttu-id="1ebd8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1ebd8-142">Int32</span></span>|<span data-ttu-id="1ebd8-143">设备计数</span><span class="sxs-lookup"><span data-stu-id="1ebd8-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="1ebd8-144">响应</span><span class="sxs-lookup"><span data-stu-id="1ebd8-144">Response</span></span>
<span data-ttu-id="1ebd8-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ebd8-146">示例</span><span class="sxs-lookup"><span data-stu-id="1ebd8-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ebd8-147">请求</span><span class="sxs-lookup"><span data-stu-id="1ebd8-147">Request</span></span>
<span data-ttu-id="1ebd8-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="1ebd8-149">响应</span><span class="sxs-lookup"><span data-stu-id="1ebd8-149">Response</span></span>
<span data-ttu-id="1ebd8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ebd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



