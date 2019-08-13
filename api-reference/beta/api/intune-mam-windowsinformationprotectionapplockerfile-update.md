---
title: 更新 windowsInformationProtectionAppLockerFile
description: 更新 windowsInformationProtectionAppLockerFile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 761b4638e261319c99be7e3135f04100de2516f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353545"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="5a8ad-103">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="5a8ad-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="5a8ad-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a8ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a8ad-106">更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-106">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a8ad-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a8ad-107">Prerequisites</span></span>
<span data-ttu-id="5a8ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a8ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a8ad-110">Permission type</span></span>|<span data-ttu-id="5a8ad-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a8ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a8ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a8ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a8ad-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a8ad-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a8ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a8ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a8ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-115">Not supported.</span></span>|
|<span data-ttu-id="5a8ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a8ad-116">Application</span></span>|<span data-ttu-id="5a8ad-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a8ad-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a8ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a8ad-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5a8ad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a8ad-119">Request headers</span></span>
|<span data-ttu-id="5a8ad-120">标头</span><span class="sxs-lookup"><span data-stu-id="5a8ad-120">Header</span></span>|<span data-ttu-id="5a8ad-121">值</span><span class="sxs-lookup"><span data-stu-id="5a8ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a8ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a8ad-122">Authorization</span></span>|<span data-ttu-id="5a8ad-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a8ad-124">接受</span><span class="sxs-lookup"><span data-stu-id="5a8ad-124">Accept</span></span>|<span data-ttu-id="5a8ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a8ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a8ad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a8ad-126">Request body</span></span>
<span data-ttu-id="5a8ad-127">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="5a8ad-128">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="5a8ad-129">属性</span><span class="sxs-lookup"><span data-stu-id="5a8ad-129">Property</span></span>|<span data-ttu-id="5a8ad-130">类型</span><span class="sxs-lookup"><span data-stu-id="5a8ad-130">Type</span></span>|<span data-ttu-id="5a8ad-131">说明</span><span class="sxs-lookup"><span data-stu-id="5a8ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a8ad-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5a8ad-132">displayName</span></span>|<span data-ttu-id="5a8ad-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5a8ad-133">String</span></span>|<span data-ttu-id="5a8ad-134">友好名称</span><span class="sxs-lookup"><span data-stu-id="5a8ad-134">The friendly name</span></span>|
|<span data-ttu-id="5a8ad-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="5a8ad-135">fileHash</span></span>|<span data-ttu-id="5a8ad-136">String</span><span class="sxs-lookup"><span data-stu-id="5a8ad-136">String</span></span>|<span data-ttu-id="5a8ad-137">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="5a8ad-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="5a8ad-138">file</span><span class="sxs-lookup"><span data-stu-id="5a8ad-138">file</span></span>|<span data-ttu-id="5a8ad-139">Binary</span><span class="sxs-lookup"><span data-stu-id="5a8ad-139">Binary</span></span>|<span data-ttu-id="5a8ad-140">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="5a8ad-140">File as a byte array</span></span>|
|<span data-ttu-id="5a8ad-141">id</span><span class="sxs-lookup"><span data-stu-id="5a8ad-141">id</span></span>|<span data-ttu-id="5a8ad-142">String</span><span class="sxs-lookup"><span data-stu-id="5a8ad-142">String</span></span>|<span data-ttu-id="5a8ad-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-143">Key of the entity.</span></span>|
|<span data-ttu-id="5a8ad-144">version</span><span class="sxs-lookup"><span data-stu-id="5a8ad-144">version</span></span>|<span data-ttu-id="5a8ad-145">String</span><span class="sxs-lookup"><span data-stu-id="5a8ad-145">String</span></span>|<span data-ttu-id="5a8ad-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5a8ad-147">响应</span><span class="sxs-lookup"><span data-stu-id="5a8ad-147">Response</span></span>
<span data-ttu-id="5a8ad-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-148">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a8ad-149">示例</span><span class="sxs-lookup"><span data-stu-id="5a8ad-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a8ad-150">请求</span><span class="sxs-lookup"><span data-stu-id="5a8ad-150">Request</span></span>
<span data-ttu-id="5a8ad-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="5a8ad-152">响应</span><span class="sxs-lookup"><span data-stu-id="5a8ad-152">Response</span></span>
<span data-ttu-id="5a8ad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a8ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






