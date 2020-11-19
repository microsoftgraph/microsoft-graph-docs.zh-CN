---
title: 更新 windowsInformationProtectionAppLearningSummary
description: 更新 windowsInformationProtectionAppLearningSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 978dce2497086fe4d13ed18d4aa966f5775ed405
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261417"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="ea92b-103">更新 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="ea92b-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="ea92b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea92b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea92b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea92b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea92b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea92b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea92b-107">更新 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea92b-107">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea92b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea92b-108">Prerequisites</span></span>
<span data-ttu-id="ea92b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea92b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea92b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea92b-111">Permission type</span></span>|<span data-ttu-id="ea92b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea92b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea92b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea92b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea92b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea92b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea92b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea92b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea92b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea92b-116">Not supported.</span></span>|
|<span data-ttu-id="ea92b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea92b-117">Application</span></span>|<span data-ttu-id="ea92b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea92b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea92b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea92b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="ea92b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea92b-120">Request headers</span></span>
|<span data-ttu-id="ea92b-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea92b-121">Header</span></span>|<span data-ttu-id="ea92b-122">值</span><span class="sxs-lookup"><span data-stu-id="ea92b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea92b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea92b-123">Authorization</span></span>|<span data-ttu-id="ea92b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea92b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea92b-125">接受</span><span class="sxs-lookup"><span data-stu-id="ea92b-125">Accept</span></span>|<span data-ttu-id="ea92b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea92b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea92b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea92b-127">Request body</span></span>
<span data-ttu-id="ea92b-128">在请求正文中，提供 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea92b-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="ea92b-129">下表显示创建 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ea92b-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="ea92b-130">属性</span><span class="sxs-lookup"><span data-stu-id="ea92b-130">Property</span></span>|<span data-ttu-id="ea92b-131">类型</span><span class="sxs-lookup"><span data-stu-id="ea92b-131">Type</span></span>|<span data-ttu-id="ea92b-132">说明</span><span class="sxs-lookup"><span data-stu-id="ea92b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea92b-133">id</span><span class="sxs-lookup"><span data-stu-id="ea92b-133">id</span></span>|<span data-ttu-id="ea92b-134">String</span><span class="sxs-lookup"><span data-stu-id="ea92b-134">String</span></span>|<span data-ttu-id="ea92b-135">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ea92b-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="ea92b-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="ea92b-136">applicationName</span></span>|<span data-ttu-id="ea92b-137">String</span><span class="sxs-lookup"><span data-stu-id="ea92b-137">String</span></span>|<span data-ttu-id="ea92b-138">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="ea92b-138">Application Name</span></span>|
|<span data-ttu-id="ea92b-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="ea92b-139">applicationType</span></span>|[<span data-ttu-id="ea92b-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="ea92b-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="ea92b-141">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="ea92b-141">Application Type.</span></span> <span data-ttu-id="ea92b-142">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="ea92b-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="ea92b-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ea92b-143">deviceCount</span></span>|<span data-ttu-id="ea92b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ea92b-144">Int32</span></span>|<span data-ttu-id="ea92b-145">设备计数</span><span class="sxs-lookup"><span data-stu-id="ea92b-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="ea92b-146">响应</span><span class="sxs-lookup"><span data-stu-id="ea92b-146">Response</span></span>
<span data-ttu-id="ea92b-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea92b-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea92b-148">示例</span><span class="sxs-lookup"><span data-stu-id="ea92b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea92b-149">请求</span><span class="sxs-lookup"><span data-stu-id="ea92b-149">Request</span></span>
<span data-ttu-id="ea92b-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea92b-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="ea92b-151">响应</span><span class="sxs-lookup"><span data-stu-id="ea92b-151">Response</span></span>
<span data-ttu-id="ea92b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea92b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




