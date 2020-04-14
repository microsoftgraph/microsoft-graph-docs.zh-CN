---
title: 更新 macOsVppAppAssignedLicense
description: 更新 macOsVppAppAssignedLicense 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8033e840c4bfda4108f97f3e7b57e52a0586fb7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406436"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="8b54c-103">更新 macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="8b54c-103">Update macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="8b54c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b54c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b54c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b54c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b54c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b54c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b54c-107">更新[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8b54c-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b54c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8b54c-108">Prerequisites</span></span>
<span data-ttu-id="8b54c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b54c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b54c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b54c-111">Permission type</span></span>|<span data-ttu-id="8b54c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8b54c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b54c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b54c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b54c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b54c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b54c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b54c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b54c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b54c-116">Not supported.</span></span>|
|<span data-ttu-id="8b54c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b54c-117">Application</span></span>|<span data-ttu-id="8b54c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b54c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b54c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b54c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="8b54c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b54c-120">Request headers</span></span>
|<span data-ttu-id="8b54c-121">标头</span><span class="sxs-lookup"><span data-stu-id="8b54c-121">Header</span></span>|<span data-ttu-id="8b54c-122">值</span><span class="sxs-lookup"><span data-stu-id="8b54c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b54c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b54c-123">Authorization</span></span>|<span data-ttu-id="8b54c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8b54c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b54c-125">接受</span><span class="sxs-lookup"><span data-stu-id="8b54c-125">Accept</span></span>|<span data-ttu-id="8b54c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b54c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b54c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b54c-127">Request body</span></span>
<span data-ttu-id="8b54c-128">在请求正文中，提供[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b54c-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="8b54c-129">下表显示创建[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8b54c-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="8b54c-130">属性</span><span class="sxs-lookup"><span data-stu-id="8b54c-130">Property</span></span>|<span data-ttu-id="8b54c-131">类型</span><span class="sxs-lookup"><span data-stu-id="8b54c-131">Type</span></span>|<span data-ttu-id="8b54c-132">说明</span><span class="sxs-lookup"><span data-stu-id="8b54c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b54c-133">id</span><span class="sxs-lookup"><span data-stu-id="8b54c-133">id</span></span>|<span data-ttu-id="8b54c-134">String</span><span class="sxs-lookup"><span data-stu-id="8b54c-134">String</span></span>|<span data-ttu-id="8b54c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b54c-135">Key of the entity.</span></span>|
|<span data-ttu-id="8b54c-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8b54c-136">userEmailAddress</span></span>|<span data-ttu-id="8b54c-137">String</span><span class="sxs-lookup"><span data-stu-id="8b54c-137">String</span></span>|<span data-ttu-id="8b54c-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8b54c-138">The user email address.</span></span>|
|<span data-ttu-id="8b54c-139">userId</span><span class="sxs-lookup"><span data-stu-id="8b54c-139">userId</span></span>|<span data-ttu-id="8b54c-140">String</span><span class="sxs-lookup"><span data-stu-id="8b54c-140">String</span></span>|<span data-ttu-id="8b54c-141">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8b54c-141">The user ID.</span></span>|
|<span data-ttu-id="8b54c-142">userName</span><span class="sxs-lookup"><span data-stu-id="8b54c-142">userName</span></span>|<span data-ttu-id="8b54c-143">String</span><span class="sxs-lookup"><span data-stu-id="8b54c-143">String</span></span>|<span data-ttu-id="8b54c-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="8b54c-144">The user name.</span></span>|
|<span data-ttu-id="8b54c-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b54c-145">userPrincipalName</span></span>|<span data-ttu-id="8b54c-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8b54c-146">String</span></span>|<span data-ttu-id="8b54c-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="8b54c-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="8b54c-148">响应</span><span class="sxs-lookup"><span data-stu-id="8b54c-148">Response</span></span>
<span data-ttu-id="8b54c-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b54c-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b54c-150">示例</span><span class="sxs-lookup"><span data-stu-id="8b54c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b54c-151">请求</span><span class="sxs-lookup"><span data-stu-id="8b54c-151">Request</span></span>
<span data-ttu-id="8b54c-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b54c-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8b54c-153">响应</span><span class="sxs-lookup"><span data-stu-id="8b54c-153">Response</span></span>
<span data-ttu-id="8b54c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b54c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```



