---
title: 创建 windowsInformationProtectionAppLearningSummary
description: 创建新的 windowsInformationProtectionAppLearningSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43f36e67ea0d1ec46708bcac1e5ecdf528f35c5b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959472"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="34cd4-103">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="34cd4-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="34cd4-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34cd4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34cd4-105">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34cd4-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34cd4-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="34cd4-106">Prerequisites</span></span>
<span data-ttu-id="34cd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34cd4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="34cd4-109">Permission type</span></span>|<span data-ttu-id="34cd4-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34cd4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34cd4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34cd4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34cd4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34cd4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="34cd4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34cd4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34cd4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="34cd4-114">Not supported.</span></span>|
|<span data-ttu-id="34cd4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="34cd4-115">Application</span></span>|<span data-ttu-id="34cd4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34cd4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34cd4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34cd4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="34cd4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="34cd4-118">Request headers</span></span>
|<span data-ttu-id="34cd4-119">标头</span><span class="sxs-lookup"><span data-stu-id="34cd4-119">Header</span></span>|<span data-ttu-id="34cd4-120">值</span><span class="sxs-lookup"><span data-stu-id="34cd4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34cd4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34cd4-121">Authorization</span></span>|<span data-ttu-id="34cd4-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34cd4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34cd4-123">接受</span><span class="sxs-lookup"><span data-stu-id="34cd4-123">Accept</span></span>|<span data-ttu-id="34cd4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34cd4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34cd4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="34cd4-125">Request body</span></span>
<span data-ttu-id="34cd4-126">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34cd4-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="34cd4-127">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="34cd4-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="34cd4-128">属性</span><span class="sxs-lookup"><span data-stu-id="34cd4-128">Property</span></span>|<span data-ttu-id="34cd4-129">类型</span><span class="sxs-lookup"><span data-stu-id="34cd4-129">Type</span></span>|<span data-ttu-id="34cd4-130">说明</span><span class="sxs-lookup"><span data-stu-id="34cd4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34cd4-131">id</span><span class="sxs-lookup"><span data-stu-id="34cd4-131">id</span></span>|<span data-ttu-id="34cd4-132">String</span><span class="sxs-lookup"><span data-stu-id="34cd4-132">String</span></span>|<span data-ttu-id="34cd4-133">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="34cd4-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="34cd4-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="34cd4-134">applicationName</span></span>|<span data-ttu-id="34cd4-135">String</span><span class="sxs-lookup"><span data-stu-id="34cd4-135">String</span></span>|<span data-ttu-id="34cd4-136">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="34cd4-136">Application Name</span></span>|
|<span data-ttu-id="34cd4-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="34cd4-137">applicationType</span></span>|[<span data-ttu-id="34cd4-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="34cd4-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="34cd4-139">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="34cd4-139">Application Type.</span></span> <span data-ttu-id="34cd4-140">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="34cd4-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="34cd4-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="34cd4-141">deviceCount</span></span>|<span data-ttu-id="34cd4-142">Int32</span><span class="sxs-lookup"><span data-stu-id="34cd4-142">Int32</span></span>|<span data-ttu-id="34cd4-143">设备计数</span><span class="sxs-lookup"><span data-stu-id="34cd4-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="34cd4-144">响应</span><span class="sxs-lookup"><span data-stu-id="34cd4-144">Response</span></span>
<span data-ttu-id="34cd4-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="34cd4-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34cd4-146">示例</span><span class="sxs-lookup"><span data-stu-id="34cd4-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="34cd4-147">请求</span><span class="sxs-lookup"><span data-stu-id="34cd4-147">Request</span></span>
<span data-ttu-id="34cd4-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34cd4-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="34cd4-149">响应</span><span class="sxs-lookup"><span data-stu-id="34cd4-149">Response</span></span>
<span data-ttu-id="34cd4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34cd4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



