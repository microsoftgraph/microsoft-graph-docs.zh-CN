---
title: 更新 windowsInformationProtectionAppLockerFile
description: 更新 windowsInformationProtectionAppLockerFile 对象的属性。
author: tfitzmac
ms.openlocfilehash: fdf14722d82da5afa2d51cb87b8e8c6ea69b9bf5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309833"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="743e2-103">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="743e2-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="743e2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="743e2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="743e2-105">更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="743e2-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="743e2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="743e2-106">Prerequisites</span></span>
<span data-ttu-id="743e2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="743e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="743e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="743e2-109">Permission type</span></span>|<span data-ttu-id="743e2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="743e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="743e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="743e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="743e2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="743e2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="743e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="743e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="743e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="743e2-114">Not supported.</span></span>|
|<span data-ttu-id="743e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="743e2-115">Application</span></span>|<span data-ttu-id="743e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="743e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="743e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="743e2-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="743e2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="743e2-118">Request headers</span></span>
|<span data-ttu-id="743e2-119">标头</span><span class="sxs-lookup"><span data-stu-id="743e2-119">Header</span></span>|<span data-ttu-id="743e2-120">值</span><span class="sxs-lookup"><span data-stu-id="743e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="743e2-121">授权</span><span class="sxs-lookup"><span data-stu-id="743e2-121">Authorization</span></span>|<span data-ttu-id="743e2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="743e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="743e2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="743e2-123">Accept</span></span>|<span data-ttu-id="743e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="743e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="743e2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="743e2-125">Request body</span></span>
<span data-ttu-id="743e2-126">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="743e2-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="743e2-127">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="743e2-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="743e2-128">属性</span><span class="sxs-lookup"><span data-stu-id="743e2-128">Property</span></span>|<span data-ttu-id="743e2-129">类型</span><span class="sxs-lookup"><span data-stu-id="743e2-129">Type</span></span>|<span data-ttu-id="743e2-130">说明</span><span class="sxs-lookup"><span data-stu-id="743e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="743e2-131">displayName</span><span class="sxs-lookup"><span data-stu-id="743e2-131">displayName</span></span>|<span data-ttu-id="743e2-132">String</span><span class="sxs-lookup"><span data-stu-id="743e2-132">String</span></span>|<span data-ttu-id="743e2-133">友好名称</span><span class="sxs-lookup"><span data-stu-id="743e2-133">The friendly name</span></span>|
|<span data-ttu-id="743e2-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="743e2-134">fileHash</span></span>|<span data-ttu-id="743e2-135">String</span><span class="sxs-lookup"><span data-stu-id="743e2-135">String</span></span>|<span data-ttu-id="743e2-136">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="743e2-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="743e2-137">file</span><span class="sxs-lookup"><span data-stu-id="743e2-137">file</span></span>|<span data-ttu-id="743e2-138">Binary</span><span class="sxs-lookup"><span data-stu-id="743e2-138">Binary</span></span>|<span data-ttu-id="743e2-139">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="743e2-139">File as a byte array</span></span>|
|<span data-ttu-id="743e2-140">id</span><span class="sxs-lookup"><span data-stu-id="743e2-140">id</span></span>|<span data-ttu-id="743e2-141">String</span><span class="sxs-lookup"><span data-stu-id="743e2-141">String</span></span>|<span data-ttu-id="743e2-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="743e2-142">Key of the entity.</span></span>|
|<span data-ttu-id="743e2-143">version</span><span class="sxs-lookup"><span data-stu-id="743e2-143">version</span></span>|<span data-ttu-id="743e2-144">String</span><span class="sxs-lookup"><span data-stu-id="743e2-144">String</span></span>|<span data-ttu-id="743e2-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="743e2-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="743e2-146">响应</span><span class="sxs-lookup"><span data-stu-id="743e2-146">Response</span></span>
<span data-ttu-id="743e2-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="743e2-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="743e2-148">示例</span><span class="sxs-lookup"><span data-stu-id="743e2-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="743e2-149">请求</span><span class="sxs-lookup"><span data-stu-id="743e2-149">Request</span></span>
<span data-ttu-id="743e2-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="743e2-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="743e2-151">响应</span><span class="sxs-lookup"><span data-stu-id="743e2-151">Response</span></span>
<span data-ttu-id="743e2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="743e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



