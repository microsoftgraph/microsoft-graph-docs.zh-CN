---
title: 更新 windowsInformationProtectionAppLearningSummary
description: 更新 windowsInformationProtectionAppLearningSummary 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20c86caed48499fc5df3a1c84254aec1ef5a4216
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360921"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="f4da6-103">更新 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="f4da6-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="f4da6-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4da6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4da6-105">更新 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4da6-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4da6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4da6-106">Prerequisites</span></span>
<span data-ttu-id="f4da6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4da6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4da6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4da6-109">Permission type</span></span>|<span data-ttu-id="f4da6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4da6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4da6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4da6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4da6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4da6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4da6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4da6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4da6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4da6-114">Not supported.</span></span>|
|<span data-ttu-id="f4da6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4da6-115">Application</span></span>|<span data-ttu-id="f4da6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4da6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4da6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4da6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f4da6-118">请求头</span><span class="sxs-lookup"><span data-stu-id="f4da6-118">Request headers</span></span>
|<span data-ttu-id="f4da6-119">标头</span><span class="sxs-lookup"><span data-stu-id="f4da6-119">Header</span></span>|<span data-ttu-id="f4da6-120">值</span><span class="sxs-lookup"><span data-stu-id="f4da6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4da6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4da6-121">Authorization</span></span>|<span data-ttu-id="f4da6-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4da6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4da6-123">接受</span><span class="sxs-lookup"><span data-stu-id="f4da6-123">Accept</span></span>|<span data-ttu-id="f4da6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f4da6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4da6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4da6-125">Request body</span></span>
<span data-ttu-id="f4da6-126">在请求正文中，提供 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4da6-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="f4da6-127">下表显示创建 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4da6-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="f4da6-128">属性</span><span class="sxs-lookup"><span data-stu-id="f4da6-128">Property</span></span>|<span data-ttu-id="f4da6-129">类型</span><span class="sxs-lookup"><span data-stu-id="f4da6-129">Type</span></span>|<span data-ttu-id="f4da6-130">说明</span><span class="sxs-lookup"><span data-stu-id="f4da6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4da6-131">id</span><span class="sxs-lookup"><span data-stu-id="f4da6-131">id</span></span>|<span data-ttu-id="f4da6-132">String</span><span class="sxs-lookup"><span data-stu-id="f4da6-132">String</span></span>|<span data-ttu-id="f4da6-133">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4da6-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="f4da6-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="f4da6-134">applicationName</span></span>|<span data-ttu-id="f4da6-135">String</span><span class="sxs-lookup"><span data-stu-id="f4da6-135">String</span></span>|<span data-ttu-id="f4da6-136">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="f4da6-136">Application Name</span></span>|
|<span data-ttu-id="f4da6-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="f4da6-137">applicationType</span></span>|[<span data-ttu-id="f4da6-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="f4da6-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="f4da6-139">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="f4da6-139">Application Type.</span></span> <span data-ttu-id="f4da6-140">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="f4da6-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="f4da6-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f4da6-141">deviceCount</span></span>|<span data-ttu-id="f4da6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f4da6-142">Int32</span></span>|<span data-ttu-id="f4da6-143">设备计数</span><span class="sxs-lookup"><span data-stu-id="f4da6-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="f4da6-144">响应</span><span class="sxs-lookup"><span data-stu-id="f4da6-144">Response</span></span>
<span data-ttu-id="f4da6-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4da6-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4da6-146">示例</span><span class="sxs-lookup"><span data-stu-id="f4da6-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4da6-147">请求</span><span class="sxs-lookup"><span data-stu-id="f4da6-147">Request</span></span>
<span data-ttu-id="f4da6-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4da6-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4da6-149">响应</span><span class="sxs-lookup"><span data-stu-id="f4da6-149">Response</span></span>
<span data-ttu-id="f4da6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4da6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




