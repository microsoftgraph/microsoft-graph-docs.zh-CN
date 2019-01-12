---
title: 更新 windowsInformationProtectionAppLockerFile
description: 更新 windowsInformationProtectionAppLockerFile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1787544bd84ca1037dafae5c26ec5f19e80fc2d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990311"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="41e0e-103">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="41e0e-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="41e0e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41e0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41e0e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41e0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41e0e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41e0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41e0e-107">更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41e0e-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41e0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41e0e-108">Prerequisites</span></span>
<span data-ttu-id="41e0e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="41e0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41e0e-111">Permission type</span></span>|<span data-ttu-id="41e0e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41e0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41e0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41e0e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e0e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41e0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41e0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41e0e-116">Not supported.</span></span>|
|<span data-ttu-id="41e0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41e0e-117">Application</span></span>|<span data-ttu-id="41e0e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="41e0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41e0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="41e0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41e0e-120">Request headers</span></span>
|<span data-ttu-id="41e0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="41e0e-121">Header</span></span>|<span data-ttu-id="41e0e-122">值</span><span class="sxs-lookup"><span data-stu-id="41e0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e0e-123">Authorization</span></span>|<span data-ttu-id="41e0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41e0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41e0e-125">Accept</span></span>|<span data-ttu-id="41e0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41e0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41e0e-127">Request body</span></span>
<span data-ttu-id="41e0e-128">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41e0e-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="41e0e-129">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41e0e-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="41e0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="41e0e-130">Property</span></span>|<span data-ttu-id="41e0e-131">类型</span><span class="sxs-lookup"><span data-stu-id="41e0e-131">Type</span></span>|<span data-ttu-id="41e0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="41e0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e0e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="41e0e-133">displayName</span></span>|<span data-ttu-id="41e0e-134">String</span><span class="sxs-lookup"><span data-stu-id="41e0e-134">String</span></span>|<span data-ttu-id="41e0e-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="41e0e-135">The friendly name</span></span>|
|<span data-ttu-id="41e0e-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="41e0e-136">fileHash</span></span>|<span data-ttu-id="41e0e-137">String</span><span class="sxs-lookup"><span data-stu-id="41e0e-137">String</span></span>|<span data-ttu-id="41e0e-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="41e0e-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="41e0e-139">file</span><span class="sxs-lookup"><span data-stu-id="41e0e-139">file</span></span>|<span data-ttu-id="41e0e-140">Binary</span><span class="sxs-lookup"><span data-stu-id="41e0e-140">Binary</span></span>|<span data-ttu-id="41e0e-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="41e0e-141">File as a byte array</span></span>|
|<span data-ttu-id="41e0e-142">id</span><span class="sxs-lookup"><span data-stu-id="41e0e-142">id</span></span>|<span data-ttu-id="41e0e-143">String</span><span class="sxs-lookup"><span data-stu-id="41e0e-143">String</span></span>|<span data-ttu-id="41e0e-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41e0e-144">Key of the entity.</span></span>|
|<span data-ttu-id="41e0e-145">version</span><span class="sxs-lookup"><span data-stu-id="41e0e-145">version</span></span>|<span data-ttu-id="41e0e-146">String</span><span class="sxs-lookup"><span data-stu-id="41e0e-146">String</span></span>|<span data-ttu-id="41e0e-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="41e0e-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="41e0e-148">响应</span><span class="sxs-lookup"><span data-stu-id="41e0e-148">Response</span></span>
<span data-ttu-id="41e0e-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41e0e-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e0e-150">示例</span><span class="sxs-lookup"><span data-stu-id="41e0e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="41e0e-151">请求</span><span class="sxs-lookup"><span data-stu-id="41e0e-151">Request</span></span>
<span data-ttu-id="41e0e-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41e0e-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 131

{
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="41e0e-153">响应</span><span class="sxs-lookup"><span data-stu-id="41e0e-153">Response</span></span>
<span data-ttu-id="41e0e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41e0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```





