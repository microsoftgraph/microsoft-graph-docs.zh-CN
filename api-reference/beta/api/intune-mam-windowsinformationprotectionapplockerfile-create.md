---
title: 创建 windowsInformationProtectionAppLockerFile
description: 创建新的 windowsInformationProtectionAppLockerFile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d5393fdbf68de218cd146817f68afbd125fa70d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987430"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="b1091-103">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="b1091-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="b1091-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1091-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1091-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1091-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1091-106">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1091-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1091-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1091-107">Prerequisites</span></span>
<span data-ttu-id="b1091-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1091-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1091-110">Permission type</span></span>|<span data-ttu-id="b1091-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1091-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1091-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1091-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1091-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1091-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1091-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1091-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1091-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1091-115">Not supported.</span></span>|
|<span data-ttu-id="b1091-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1091-116">Application</span></span>|<span data-ttu-id="b1091-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1091-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1091-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1091-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b1091-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1091-119">Request headers</span></span>
|<span data-ttu-id="b1091-120">标头</span><span class="sxs-lookup"><span data-stu-id="b1091-120">Header</span></span>|<span data-ttu-id="b1091-121">值</span><span class="sxs-lookup"><span data-stu-id="b1091-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1091-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1091-122">Authorization</span></span>|<span data-ttu-id="b1091-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1091-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1091-124">接受</span><span class="sxs-lookup"><span data-stu-id="b1091-124">Accept</span></span>|<span data-ttu-id="b1091-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1091-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1091-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1091-126">Request body</span></span>
<span data-ttu-id="b1091-127">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1091-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="b1091-128">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1091-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="b1091-129">属性</span><span class="sxs-lookup"><span data-stu-id="b1091-129">Property</span></span>|<span data-ttu-id="b1091-130">类型</span><span class="sxs-lookup"><span data-stu-id="b1091-130">Type</span></span>|<span data-ttu-id="b1091-131">说明</span><span class="sxs-lookup"><span data-stu-id="b1091-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1091-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b1091-132">displayName</span></span>|<span data-ttu-id="b1091-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b1091-133">String</span></span>|<span data-ttu-id="b1091-134">友好名称</span><span class="sxs-lookup"><span data-stu-id="b1091-134">The friendly name</span></span>|
|<span data-ttu-id="b1091-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="b1091-135">fileHash</span></span>|<span data-ttu-id="b1091-136">String</span><span class="sxs-lookup"><span data-stu-id="b1091-136">String</span></span>|<span data-ttu-id="b1091-137">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="b1091-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="b1091-138">file</span><span class="sxs-lookup"><span data-stu-id="b1091-138">file</span></span>|<span data-ttu-id="b1091-139">Binary</span><span class="sxs-lookup"><span data-stu-id="b1091-139">Binary</span></span>|<span data-ttu-id="b1091-140">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="b1091-140">File as a byte array</span></span>|
|<span data-ttu-id="b1091-141">id</span><span class="sxs-lookup"><span data-stu-id="b1091-141">id</span></span>|<span data-ttu-id="b1091-142">String</span><span class="sxs-lookup"><span data-stu-id="b1091-142">String</span></span>|<span data-ttu-id="b1091-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1091-143">Key of the entity.</span></span>|
|<span data-ttu-id="b1091-144">version</span><span class="sxs-lookup"><span data-stu-id="b1091-144">version</span></span>|<span data-ttu-id="b1091-145">String</span><span class="sxs-lookup"><span data-stu-id="b1091-145">String</span></span>|<span data-ttu-id="b1091-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b1091-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b1091-147">响应</span><span class="sxs-lookup"><span data-stu-id="b1091-147">Response</span></span>
<span data-ttu-id="b1091-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1091-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1091-149">示例</span><span class="sxs-lookup"><span data-stu-id="b1091-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1091-150">请求</span><span class="sxs-lookup"><span data-stu-id="b1091-150">Request</span></span>
<span data-ttu-id="b1091-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1091-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1091-152">响应</span><span class="sxs-lookup"><span data-stu-id="b1091-152">Response</span></span>
<span data-ttu-id="b1091-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1091-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





