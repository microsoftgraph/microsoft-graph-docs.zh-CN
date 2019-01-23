---
title: 更新 windowsInformationProtectionAppLockerFile
description: 更新 windowsInformationProtectionAppLockerFile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eee21cf2a7f2ece277ab3435b566d486120a8fc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399827"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="0412b-103">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="0412b-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="0412b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0412b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0412b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0412b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0412b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0412b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0412b-107">更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0412b-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0412b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0412b-108">Prerequisites</span></span>
<span data-ttu-id="0412b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0412b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0412b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0412b-111">Permission type</span></span>|<span data-ttu-id="0412b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0412b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0412b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0412b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0412b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0412b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0412b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0412b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0412b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0412b-116">Not supported.</span></span>|
|<span data-ttu-id="0412b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0412b-117">Application</span></span>|<span data-ttu-id="0412b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0412b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0412b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0412b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0412b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0412b-120">Request headers</span></span>
|<span data-ttu-id="0412b-121">标头</span><span class="sxs-lookup"><span data-stu-id="0412b-121">Header</span></span>|<span data-ttu-id="0412b-122">值</span><span class="sxs-lookup"><span data-stu-id="0412b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0412b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0412b-123">Authorization</span></span>|<span data-ttu-id="0412b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0412b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0412b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0412b-125">Accept</span></span>|<span data-ttu-id="0412b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0412b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0412b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0412b-127">Request body</span></span>
<span data-ttu-id="0412b-128">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0412b-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="0412b-129">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0412b-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="0412b-130">属性</span><span class="sxs-lookup"><span data-stu-id="0412b-130">Property</span></span>|<span data-ttu-id="0412b-131">类型</span><span class="sxs-lookup"><span data-stu-id="0412b-131">Type</span></span>|<span data-ttu-id="0412b-132">说明</span><span class="sxs-lookup"><span data-stu-id="0412b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0412b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0412b-133">displayName</span></span>|<span data-ttu-id="0412b-134">String</span><span class="sxs-lookup"><span data-stu-id="0412b-134">String</span></span>|<span data-ttu-id="0412b-135">友好名称</span><span class="sxs-lookup"><span data-stu-id="0412b-135">The friendly name</span></span>|
|<span data-ttu-id="0412b-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="0412b-136">fileHash</span></span>|<span data-ttu-id="0412b-137">String</span><span class="sxs-lookup"><span data-stu-id="0412b-137">String</span></span>|<span data-ttu-id="0412b-138">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="0412b-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="0412b-139">file</span><span class="sxs-lookup"><span data-stu-id="0412b-139">file</span></span>|<span data-ttu-id="0412b-140">Binary</span><span class="sxs-lookup"><span data-stu-id="0412b-140">Binary</span></span>|<span data-ttu-id="0412b-141">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="0412b-141">File as a byte array</span></span>|
|<span data-ttu-id="0412b-142">id</span><span class="sxs-lookup"><span data-stu-id="0412b-142">id</span></span>|<span data-ttu-id="0412b-143">String</span><span class="sxs-lookup"><span data-stu-id="0412b-143">String</span></span>|<span data-ttu-id="0412b-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0412b-144">Key of the entity.</span></span>|
|<span data-ttu-id="0412b-145">version</span><span class="sxs-lookup"><span data-stu-id="0412b-145">version</span></span>|<span data-ttu-id="0412b-146">String</span><span class="sxs-lookup"><span data-stu-id="0412b-146">String</span></span>|<span data-ttu-id="0412b-147">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="0412b-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0412b-148">响应</span><span class="sxs-lookup"><span data-stu-id="0412b-148">Response</span></span>
<span data-ttu-id="0412b-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0412b-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0412b-150">示例</span><span class="sxs-lookup"><span data-stu-id="0412b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0412b-151">请求</span><span class="sxs-lookup"><span data-stu-id="0412b-151">Request</span></span>
<span data-ttu-id="0412b-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0412b-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0412b-153">响应</span><span class="sxs-lookup"><span data-stu-id="0412b-153">Response</span></span>
<span data-ttu-id="0412b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0412b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




