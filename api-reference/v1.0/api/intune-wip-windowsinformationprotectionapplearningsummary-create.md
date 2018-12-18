---
title: 创建 windowsInformationProtectionAppLearningSummary
description: 创建新的 windowsInformationProtectionAppLearningSummary 对象。
author: tfitzmac
ms.openlocfilehash: fdcf4be10f26036c06f4cfd0a67f98601c296ec7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354297"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="5d6bc-103">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="5d6bc-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="5d6bc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d6bc-105">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d6bc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5d6bc-106">Prerequisites</span></span>
<span data-ttu-id="5d6bc-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5d6bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d6bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d6bc-109">Permission type</span></span>|<span data-ttu-id="5d6bc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d6bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d6bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d6bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d6bc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d6bc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d6bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d6bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d6bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-114">Not supported.</span></span>|
|<span data-ttu-id="5d6bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d6bc-115">Application</span></span>|<span data-ttu-id="5d6bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d6bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d6bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5d6bc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d6bc-118">Request headers</span></span>
|<span data-ttu-id="5d6bc-119">标头</span><span class="sxs-lookup"><span data-stu-id="5d6bc-119">Header</span></span>|<span data-ttu-id="5d6bc-120">值</span><span class="sxs-lookup"><span data-stu-id="5d6bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d6bc-121">授权</span><span class="sxs-lookup"><span data-stu-id="5d6bc-121">Authorization</span></span>|<span data-ttu-id="5d6bc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d6bc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5d6bc-123">Accept</span></span>|<span data-ttu-id="5d6bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5d6bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d6bc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d6bc-125">Request body</span></span>
<span data-ttu-id="5d6bc-126">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="5d6bc-127">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="5d6bc-128">属性</span><span class="sxs-lookup"><span data-stu-id="5d6bc-128">Property</span></span>|<span data-ttu-id="5d6bc-129">类型</span><span class="sxs-lookup"><span data-stu-id="5d6bc-129">Type</span></span>|<span data-ttu-id="5d6bc-130">说明</span><span class="sxs-lookup"><span data-stu-id="5d6bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d6bc-131">id</span><span class="sxs-lookup"><span data-stu-id="5d6bc-131">id</span></span>|<span data-ttu-id="5d6bc-132">String</span><span class="sxs-lookup"><span data-stu-id="5d6bc-132">String</span></span>|<span data-ttu-id="5d6bc-133">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="5d6bc-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="5d6bc-134">applicationName</span></span>|<span data-ttu-id="5d6bc-135">String</span><span class="sxs-lookup"><span data-stu-id="5d6bc-135">String</span></span>|<span data-ttu-id="5d6bc-136">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="5d6bc-136">Application Name</span></span>|
|<span data-ttu-id="5d6bc-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="5d6bc-137">applicationType</span></span>|[<span data-ttu-id="5d6bc-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="5d6bc-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="5d6bc-139">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-139">Application Type.</span></span> <span data-ttu-id="5d6bc-140">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="5d6bc-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5d6bc-141">deviceCount</span></span>|<span data-ttu-id="5d6bc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6bc-142">Int32</span></span>|<span data-ttu-id="5d6bc-143">设备计数</span><span class="sxs-lookup"><span data-stu-id="5d6bc-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="5d6bc-144">响应</span><span class="sxs-lookup"><span data-stu-id="5d6bc-144">Response</span></span>
<span data-ttu-id="5d6bc-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d6bc-146">示例</span><span class="sxs-lookup"><span data-stu-id="5d6bc-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d6bc-147">请求</span><span class="sxs-lookup"><span data-stu-id="5d6bc-147">Request</span></span>
<span data-ttu-id="5d6bc-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d6bc-149">响应</span><span class="sxs-lookup"><span data-stu-id="5d6bc-149">Response</span></span>
<span data-ttu-id="5d6bc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d6bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



