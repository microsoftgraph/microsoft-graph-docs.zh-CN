---
title: 更新 windowsInformationProtectionAppLockerFile
description: 更新 windowsInformationProtectionAppLockerFile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6d81b953288e1c8c9435a9502616f3f9fbc1d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923822"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="ece38-103">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="ece38-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="ece38-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ece38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ece38-105">更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ece38-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ece38-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ece38-106">Prerequisites</span></span>
<span data-ttu-id="ece38-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ece38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ece38-109">Permission type</span></span>|<span data-ttu-id="ece38-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ece38-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ece38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ece38-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece38-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ece38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ece38-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece38-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ece38-114">Not supported.</span></span>|
|<span data-ttu-id="ece38-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ece38-115">Application</span></span>|<span data-ttu-id="ece38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ece38-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ece38-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ece38-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ece38-118">Request headers</span></span>
|<span data-ttu-id="ece38-119">标头</span><span class="sxs-lookup"><span data-stu-id="ece38-119">Header</span></span>|<span data-ttu-id="ece38-120">值</span><span class="sxs-lookup"><span data-stu-id="ece38-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece38-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ece38-121">Authorization</span></span>|<span data-ttu-id="ece38-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ece38-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece38-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ece38-123">Accept</span></span>|<span data-ttu-id="ece38-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ece38-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece38-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ece38-125">Request body</span></span>
<span data-ttu-id="ece38-126">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ece38-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="ece38-127">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ece38-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="ece38-128">属性</span><span class="sxs-lookup"><span data-stu-id="ece38-128">Property</span></span>|<span data-ttu-id="ece38-129">类型</span><span class="sxs-lookup"><span data-stu-id="ece38-129">Type</span></span>|<span data-ttu-id="ece38-130">说明</span><span class="sxs-lookup"><span data-stu-id="ece38-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ece38-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ece38-131">displayName</span></span>|<span data-ttu-id="ece38-132">String</span><span class="sxs-lookup"><span data-stu-id="ece38-132">String</span></span>|<span data-ttu-id="ece38-133">友好名称</span><span class="sxs-lookup"><span data-stu-id="ece38-133">The friendly name</span></span>|
|<span data-ttu-id="ece38-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="ece38-134">fileHash</span></span>|<span data-ttu-id="ece38-135">String</span><span class="sxs-lookup"><span data-stu-id="ece38-135">String</span></span>|<span data-ttu-id="ece38-136">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="ece38-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="ece38-137">file</span><span class="sxs-lookup"><span data-stu-id="ece38-137">file</span></span>|<span data-ttu-id="ece38-138">Binary</span><span class="sxs-lookup"><span data-stu-id="ece38-138">Binary</span></span>|<span data-ttu-id="ece38-139">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="ece38-139">File as a byte array</span></span>|
|<span data-ttu-id="ece38-140">id</span><span class="sxs-lookup"><span data-stu-id="ece38-140">id</span></span>|<span data-ttu-id="ece38-141">String</span><span class="sxs-lookup"><span data-stu-id="ece38-141">String</span></span>|<span data-ttu-id="ece38-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ece38-142">Key of the entity.</span></span>|
|<span data-ttu-id="ece38-143">version</span><span class="sxs-lookup"><span data-stu-id="ece38-143">version</span></span>|<span data-ttu-id="ece38-144">String</span><span class="sxs-lookup"><span data-stu-id="ece38-144">String</span></span>|<span data-ttu-id="ece38-145">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="ece38-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ece38-146">响应</span><span class="sxs-lookup"><span data-stu-id="ece38-146">Response</span></span>
<span data-ttu-id="ece38-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ece38-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece38-148">示例</span><span class="sxs-lookup"><span data-stu-id="ece38-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="ece38-149">请求</span><span class="sxs-lookup"><span data-stu-id="ece38-149">Request</span></span>
<span data-ttu-id="ece38-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ece38-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ece38-151">响应</span><span class="sxs-lookup"><span data-stu-id="ece38-151">Response</span></span>
<span data-ttu-id="ece38-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ece38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



