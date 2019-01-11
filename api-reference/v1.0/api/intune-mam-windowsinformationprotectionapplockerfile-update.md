---
title: 更新 windowsInformationProtectionAppLockerFile
description: 更新 windowsInformationProtectionAppLockerFile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 59b5fef4b2fd82f1275e14321c46aec0130ddb9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826185"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="2df52-103">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="2df52-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="2df52-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2df52-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df52-105">更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2df52-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df52-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2df52-106">Prerequisites</span></span>
<span data-ttu-id="2df52-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2df52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df52-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2df52-109">Permission type</span></span>|<span data-ttu-id="2df52-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2df52-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df52-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2df52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2df52-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df52-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2df52-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2df52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df52-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df52-114">Not supported.</span></span>|
|<span data-ttu-id="2df52-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2df52-115">Application</span></span>|<span data-ttu-id="2df52-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df52-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2df52-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2df52-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2df52-118">Request headers</span></span>
|<span data-ttu-id="2df52-119">标头</span><span class="sxs-lookup"><span data-stu-id="2df52-119">Header</span></span>|<span data-ttu-id="2df52-120">值</span><span class="sxs-lookup"><span data-stu-id="2df52-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df52-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df52-121">Authorization</span></span>|<span data-ttu-id="2df52-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2df52-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df52-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2df52-123">Accept</span></span>|<span data-ttu-id="2df52-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2df52-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df52-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2df52-125">Request body</span></span>
<span data-ttu-id="2df52-126">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2df52-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="2df52-127">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2df52-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="2df52-128">属性</span><span class="sxs-lookup"><span data-stu-id="2df52-128">Property</span></span>|<span data-ttu-id="2df52-129">类型</span><span class="sxs-lookup"><span data-stu-id="2df52-129">Type</span></span>|<span data-ttu-id="2df52-130">说明</span><span class="sxs-lookup"><span data-stu-id="2df52-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df52-131">displayName</span><span class="sxs-lookup"><span data-stu-id="2df52-131">displayName</span></span>|<span data-ttu-id="2df52-132">String</span><span class="sxs-lookup"><span data-stu-id="2df52-132">String</span></span>|<span data-ttu-id="2df52-133">友好名称</span><span class="sxs-lookup"><span data-stu-id="2df52-133">The friendly name</span></span>|
|<span data-ttu-id="2df52-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="2df52-134">fileHash</span></span>|<span data-ttu-id="2df52-135">String</span><span class="sxs-lookup"><span data-stu-id="2df52-135">String</span></span>|<span data-ttu-id="2df52-136">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="2df52-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="2df52-137">file</span><span class="sxs-lookup"><span data-stu-id="2df52-137">file</span></span>|<span data-ttu-id="2df52-138">Binary</span><span class="sxs-lookup"><span data-stu-id="2df52-138">Binary</span></span>|<span data-ttu-id="2df52-139">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="2df52-139">File as a byte array</span></span>|
|<span data-ttu-id="2df52-140">id</span><span class="sxs-lookup"><span data-stu-id="2df52-140">id</span></span>|<span data-ttu-id="2df52-141">String</span><span class="sxs-lookup"><span data-stu-id="2df52-141">String</span></span>|<span data-ttu-id="2df52-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2df52-142">Key of the entity.</span></span>|
|<span data-ttu-id="2df52-143">version</span><span class="sxs-lookup"><span data-stu-id="2df52-143">version</span></span>|<span data-ttu-id="2df52-144">String</span><span class="sxs-lookup"><span data-stu-id="2df52-144">String</span></span>|<span data-ttu-id="2df52-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="2df52-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2df52-146">响应</span><span class="sxs-lookup"><span data-stu-id="2df52-146">Response</span></span>
<span data-ttu-id="2df52-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2df52-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df52-148">示例</span><span class="sxs-lookup"><span data-stu-id="2df52-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df52-149">请求</span><span class="sxs-lookup"><span data-stu-id="2df52-149">Request</span></span>
<span data-ttu-id="2df52-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2df52-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="2df52-151">响应</span><span class="sxs-lookup"><span data-stu-id="2df52-151">Response</span></span>
<span data-ttu-id="2df52-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2df52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



