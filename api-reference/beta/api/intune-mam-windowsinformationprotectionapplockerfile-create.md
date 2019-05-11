---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad14be8ae66c48a66899d9ab8c5590d847aa7a77
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33902960"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="89700-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="89700-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="89700-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89700-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89700-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89700-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89700-106">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89700-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89700-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="89700-107">Prerequisites</span></span>
<span data-ttu-id="89700-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89700-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89700-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="89700-110">Permission type</span></span>|<span data-ttu-id="89700-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89700-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89700-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89700-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89700-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89700-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89700-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89700-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89700-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="89700-115">Not supported.</span></span>|
|<span data-ttu-id="89700-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="89700-116">Application</span></span>|<span data-ttu-id="89700-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="89700-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89700-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89700-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="89700-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="89700-119">Request headers</span></span>
|<span data-ttu-id="89700-120">标头</span><span class="sxs-lookup"><span data-stu-id="89700-120">Header</span></span>|<span data-ttu-id="89700-121">值</span><span class="sxs-lookup"><span data-stu-id="89700-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89700-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89700-122">Authorization</span></span>|<span data-ttu-id="89700-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89700-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89700-124">接受</span><span class="sxs-lookup"><span data-stu-id="89700-124">Accept</span></span>|<span data-ttu-id="89700-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89700-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89700-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="89700-126">Request body</span></span>
<span data-ttu-id="89700-127">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89700-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="89700-128">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89700-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="89700-129">属性</span><span class="sxs-lookup"><span data-stu-id="89700-129">Property</span></span>|<span data-ttu-id="89700-130">类型</span><span class="sxs-lookup"><span data-stu-id="89700-130">Type</span></span>|<span data-ttu-id="89700-131">说明</span><span class="sxs-lookup"><span data-stu-id="89700-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89700-132">displayName</span><span class="sxs-lookup"><span data-stu-id="89700-132">displayName</span></span>|<span data-ttu-id="89700-133">字符串</span><span class="sxs-lookup"><span data-stu-id="89700-133">String</span></span>|<span data-ttu-id="89700-134">友好名称</span><span class="sxs-lookup"><span data-stu-id="89700-134">The friendly name</span></span>|
|<span data-ttu-id="89700-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="89700-135">fileHash</span></span>|<span data-ttu-id="89700-136">String</span><span class="sxs-lookup"><span data-stu-id="89700-136">String</span></span>|<span data-ttu-id="89700-137">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="89700-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="89700-138">file</span><span class="sxs-lookup"><span data-stu-id="89700-138">file</span></span>|<span data-ttu-id="89700-139">Binary</span><span class="sxs-lookup"><span data-stu-id="89700-139">Binary</span></span>|<span data-ttu-id="89700-140">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="89700-140">File as a byte array</span></span>|
|<span data-ttu-id="89700-141">id</span><span class="sxs-lookup"><span data-stu-id="89700-141">id</span></span>|<span data-ttu-id="89700-142">String</span><span class="sxs-lookup"><span data-stu-id="89700-142">String</span></span>|<span data-ttu-id="89700-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="89700-143">Key of the entity.</span></span>|
|<span data-ttu-id="89700-144">version</span><span class="sxs-lookup"><span data-stu-id="89700-144">version</span></span>|<span data-ttu-id="89700-145">String</span><span class="sxs-lookup"><span data-stu-id="89700-145">String</span></span>|<span data-ttu-id="89700-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="89700-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="89700-147">响应</span><span class="sxs-lookup"><span data-stu-id="89700-147">Response</span></span>
<span data-ttu-id="89700-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89700-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89700-149">示例</span><span class="sxs-lookup"><span data-stu-id="89700-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="89700-150">请求</span><span class="sxs-lookup"><span data-stu-id="89700-150">Request</span></span>
<span data-ttu-id="89700-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89700-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="89700-152">响应</span><span class="sxs-lookup"><span data-stu-id="89700-152">Response</span></span>
<span data-ttu-id="89700-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89700-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




