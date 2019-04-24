---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22e4be6d282ba7750b6c896b2592ea8b0b71a62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453565"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="74348-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="74348-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="74348-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74348-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74348-105">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74348-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74348-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="74348-106">Prerequisites</span></span>
<span data-ttu-id="74348-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74348-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="74348-109">Permission type</span></span>|<span data-ttu-id="74348-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74348-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74348-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74348-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74348-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74348-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74348-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74348-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74348-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="74348-114">Not supported.</span></span>|
|<span data-ttu-id="74348-115">Application</span><span class="sxs-lookup"><span data-stu-id="74348-115">Application</span></span>|<span data-ttu-id="74348-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74348-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74348-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74348-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="74348-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="74348-118">Request headers</span></span>
|<span data-ttu-id="74348-119">标头</span><span class="sxs-lookup"><span data-stu-id="74348-119">Header</span></span>|<span data-ttu-id="74348-120">值</span><span class="sxs-lookup"><span data-stu-id="74348-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74348-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74348-121">Authorization</span></span>|<span data-ttu-id="74348-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74348-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74348-123">接受</span><span class="sxs-lookup"><span data-stu-id="74348-123">Accept</span></span>|<span data-ttu-id="74348-124">application/json</span><span class="sxs-lookup"><span data-stu-id="74348-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74348-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="74348-125">Request body</span></span>
<span data-ttu-id="74348-126">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74348-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="74348-127">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74348-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="74348-128">属性</span><span class="sxs-lookup"><span data-stu-id="74348-128">Property</span></span>|<span data-ttu-id="74348-129">类型</span><span class="sxs-lookup"><span data-stu-id="74348-129">Type</span></span>|<span data-ttu-id="74348-130">说明</span><span class="sxs-lookup"><span data-stu-id="74348-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74348-131">displayName</span><span class="sxs-lookup"><span data-stu-id="74348-131">displayName</span></span>|<span data-ttu-id="74348-132">字符串</span><span class="sxs-lookup"><span data-stu-id="74348-132">String</span></span>|<span data-ttu-id="74348-133">友好名称</span><span class="sxs-lookup"><span data-stu-id="74348-133">The friendly name</span></span>|
|<span data-ttu-id="74348-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="74348-134">fileHash</span></span>|<span data-ttu-id="74348-135">String</span><span class="sxs-lookup"><span data-stu-id="74348-135">String</span></span>|<span data-ttu-id="74348-136">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="74348-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="74348-137">file</span><span class="sxs-lookup"><span data-stu-id="74348-137">file</span></span>|<span data-ttu-id="74348-138">Binary</span><span class="sxs-lookup"><span data-stu-id="74348-138">Binary</span></span>|<span data-ttu-id="74348-139">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="74348-139">File as a byte array</span></span>|
|<span data-ttu-id="74348-140">id</span><span class="sxs-lookup"><span data-stu-id="74348-140">id</span></span>|<span data-ttu-id="74348-141">String</span><span class="sxs-lookup"><span data-stu-id="74348-141">String</span></span>|<span data-ttu-id="74348-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74348-142">Key of the entity.</span></span>|
|<span data-ttu-id="74348-143">version</span><span class="sxs-lookup"><span data-stu-id="74348-143">version</span></span>|<span data-ttu-id="74348-144">字符串</span><span class="sxs-lookup"><span data-stu-id="74348-144">String</span></span>|<span data-ttu-id="74348-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="74348-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="74348-146">响应</span><span class="sxs-lookup"><span data-stu-id="74348-146">Response</span></span>
<span data-ttu-id="74348-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74348-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74348-148">示例</span><span class="sxs-lookup"><span data-stu-id="74348-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="74348-149">请求</span><span class="sxs-lookup"><span data-stu-id="74348-149">Request</span></span>
<span data-ttu-id="74348-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74348-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="74348-151">响应</span><span class="sxs-lookup"><span data-stu-id="74348-151">Response</span></span>
<span data-ttu-id="74348-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74348-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



