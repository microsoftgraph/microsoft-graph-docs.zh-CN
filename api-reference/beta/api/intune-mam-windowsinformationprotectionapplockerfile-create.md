---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aca3b775053e8f240382274fc6bb62c6b602a113
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462976"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="b540d-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="b540d-103">Create windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="b540d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b540d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b540d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b540d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b540d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b540d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b540d-107">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b540d-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b540d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b540d-108">Prerequisites</span></span>
<span data-ttu-id="b540d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b540d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b540d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b540d-111">Permission type</span></span>|<span data-ttu-id="b540d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b540d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b540d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b540d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b540d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b540d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b540d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b540d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b540d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b540d-116">Not supported.</span></span>|
|<span data-ttu-id="b540d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b540d-117">Application</span></span>|<span data-ttu-id="b540d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b540d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b540d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b540d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b540d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b540d-120">Request headers</span></span>
|<span data-ttu-id="b540d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b540d-121">Header</span></span>|<span data-ttu-id="b540d-122">值</span><span class="sxs-lookup"><span data-stu-id="b540d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b540d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b540d-123">Authorization</span></span>|<span data-ttu-id="b540d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b540d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b540d-125">接受</span><span class="sxs-lookup"><span data-stu-id="b540d-125">Accept</span></span>|<span data-ttu-id="b540d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b540d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b540d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b540d-127">Request body</span></span>
<span data-ttu-id="b540d-128">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b540d-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="b540d-129">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b540d-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="b540d-130">属性</span><span class="sxs-lookup"><span data-stu-id="b540d-130">Property</span></span>|<span data-ttu-id="b540d-131">类型</span><span class="sxs-lookup"><span data-stu-id="b540d-131">Type</span></span>|<span data-ttu-id="b540d-132">说明</span><span class="sxs-lookup"><span data-stu-id="b540d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b540d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b540d-133">displayName</span></span>|<span data-ttu-id="b540d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b540d-134">String</span></span>|<span data-ttu-id="b540d-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="b540d-135">The friendly name</span></span>|
|<span data-ttu-id="b540d-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="b540d-136">fileHash</span></span>|<span data-ttu-id="b540d-137">String</span><span class="sxs-lookup"><span data-stu-id="b540d-137">String</span></span>|<span data-ttu-id="b540d-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="b540d-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="b540d-139">file</span><span class="sxs-lookup"><span data-stu-id="b540d-139">file</span></span>|<span data-ttu-id="b540d-140">Binary</span><span class="sxs-lookup"><span data-stu-id="b540d-140">Binary</span></span>|<span data-ttu-id="b540d-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="b540d-141">File as a byte array</span></span>|
|<span data-ttu-id="b540d-142">id</span><span class="sxs-lookup"><span data-stu-id="b540d-142">id</span></span>|<span data-ttu-id="b540d-143">String</span><span class="sxs-lookup"><span data-stu-id="b540d-143">String</span></span>|<span data-ttu-id="b540d-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b540d-144">Key of the entity.</span></span>|
|<span data-ttu-id="b540d-145">version</span><span class="sxs-lookup"><span data-stu-id="b540d-145">version</span></span>|<span data-ttu-id="b540d-146">String</span><span class="sxs-lookup"><span data-stu-id="b540d-146">String</span></span>|<span data-ttu-id="b540d-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b540d-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b540d-148">响应</span><span class="sxs-lookup"><span data-stu-id="b540d-148">Response</span></span>
<span data-ttu-id="b540d-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b540d-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b540d-150">示例</span><span class="sxs-lookup"><span data-stu-id="b540d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b540d-151">请求</span><span class="sxs-lookup"><span data-stu-id="b540d-151">Request</span></span>
<span data-ttu-id="b540d-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b540d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b540d-153">响应</span><span class="sxs-lookup"><span data-stu-id="b540d-153">Response</span></span>
<span data-ttu-id="b540d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b540d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





