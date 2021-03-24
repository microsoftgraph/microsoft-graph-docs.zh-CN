---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 576e6a284c65cfe9e21aae1f33ce7ed50e56183e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148874"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="68afc-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="68afc-103">Create windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="68afc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68afc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68afc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68afc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68afc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68afc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68afc-107">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68afc-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68afc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="68afc-108">Prerequisites</span></span>
<span data-ttu-id="68afc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68afc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="68afc-111">Permission type</span></span>|<span data-ttu-id="68afc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68afc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68afc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68afc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68afc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68afc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68afc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68afc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68afc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="68afc-116">Not supported.</span></span>|
|<span data-ttu-id="68afc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="68afc-117">Application</span></span>|<span data-ttu-id="68afc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68afc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68afc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68afc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="68afc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="68afc-120">Request headers</span></span>
|<span data-ttu-id="68afc-121">标头</span><span class="sxs-lookup"><span data-stu-id="68afc-121">Header</span></span>|<span data-ttu-id="68afc-122">值</span><span class="sxs-lookup"><span data-stu-id="68afc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68afc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68afc-123">Authorization</span></span>|<span data-ttu-id="68afc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="68afc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68afc-125">接受</span><span class="sxs-lookup"><span data-stu-id="68afc-125">Accept</span></span>|<span data-ttu-id="68afc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68afc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68afc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="68afc-127">Request body</span></span>
<span data-ttu-id="68afc-128">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68afc-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="68afc-129">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="68afc-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="68afc-130">属性</span><span class="sxs-lookup"><span data-stu-id="68afc-130">Property</span></span>|<span data-ttu-id="68afc-131">类型</span><span class="sxs-lookup"><span data-stu-id="68afc-131">Type</span></span>|<span data-ttu-id="68afc-132">说明</span><span class="sxs-lookup"><span data-stu-id="68afc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68afc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="68afc-133">displayName</span></span>|<span data-ttu-id="68afc-134">String</span><span class="sxs-lookup"><span data-stu-id="68afc-134">String</span></span>|<span data-ttu-id="68afc-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="68afc-135">The friendly name</span></span>|
|<span data-ttu-id="68afc-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="68afc-136">fileHash</span></span>|<span data-ttu-id="68afc-137">String</span><span class="sxs-lookup"><span data-stu-id="68afc-137">String</span></span>|<span data-ttu-id="68afc-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="68afc-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="68afc-139">file</span><span class="sxs-lookup"><span data-stu-id="68afc-139">file</span></span>|<span data-ttu-id="68afc-140">Binary</span><span class="sxs-lookup"><span data-stu-id="68afc-140">Binary</span></span>|<span data-ttu-id="68afc-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="68afc-141">File as a byte array</span></span>|
|<span data-ttu-id="68afc-142">id</span><span class="sxs-lookup"><span data-stu-id="68afc-142">id</span></span>|<span data-ttu-id="68afc-143">String</span><span class="sxs-lookup"><span data-stu-id="68afc-143">String</span></span>|<span data-ttu-id="68afc-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="68afc-144">Key of the entity.</span></span>|
|<span data-ttu-id="68afc-145">version</span><span class="sxs-lookup"><span data-stu-id="68afc-145">version</span></span>|<span data-ttu-id="68afc-146">String</span><span class="sxs-lookup"><span data-stu-id="68afc-146">String</span></span>|<span data-ttu-id="68afc-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="68afc-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="68afc-148">响应</span><span class="sxs-lookup"><span data-stu-id="68afc-148">Response</span></span>
<span data-ttu-id="68afc-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68afc-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68afc-150">示例</span><span class="sxs-lookup"><span data-stu-id="68afc-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="68afc-151">请求</span><span class="sxs-lookup"><span data-stu-id="68afc-151">Request</span></span>
<span data-ttu-id="68afc-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68afc-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68afc-153">响应</span><span class="sxs-lookup"><span data-stu-id="68afc-153">Response</span></span>
<span data-ttu-id="68afc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68afc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




