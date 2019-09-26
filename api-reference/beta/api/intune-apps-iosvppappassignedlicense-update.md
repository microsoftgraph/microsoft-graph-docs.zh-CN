---
title: 更新 iosVppAppAssignedLicense
description: 更新 iosVppAppAssignedLicense 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d77fd9f381159cd4504c8c4480d3eafd5790533
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173442"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="fd449-103">更新 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="fd449-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="fd449-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd449-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd449-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd449-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd449-106">更新[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd449-106">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd449-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd449-107">Prerequisites</span></span>
<span data-ttu-id="fd449-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd449-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd449-110">Permission type</span></span>|<span data-ttu-id="fd449-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd449-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd449-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd449-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd449-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd449-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd449-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd449-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd449-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd449-115">Not supported.</span></span>|
|<span data-ttu-id="fd449-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd449-116">Application</span></span>|<span data-ttu-id="fd449-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd449-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd449-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd449-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="fd449-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd449-119">Request headers</span></span>
|<span data-ttu-id="fd449-120">标头</span><span class="sxs-lookup"><span data-stu-id="fd449-120">Header</span></span>|<span data-ttu-id="fd449-121">值</span><span class="sxs-lookup"><span data-stu-id="fd449-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd449-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd449-122">Authorization</span></span>|<span data-ttu-id="fd449-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd449-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd449-124">接受</span><span class="sxs-lookup"><span data-stu-id="fd449-124">Accept</span></span>|<span data-ttu-id="fd449-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd449-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd449-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd449-126">Request body</span></span>
<span data-ttu-id="fd449-127">在请求正文中，提供[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd449-127">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="fd449-128">下表显示创建[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fd449-128">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="fd449-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd449-129">Property</span></span>|<span data-ttu-id="fd449-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd449-130">Type</span></span>|<span data-ttu-id="fd449-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd449-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd449-132">id</span><span class="sxs-lookup"><span data-stu-id="fd449-132">id</span></span>|<span data-ttu-id="fd449-133">String</span><span class="sxs-lookup"><span data-stu-id="fd449-133">String</span></span>|<span data-ttu-id="fd449-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fd449-134">Key of the entity.</span></span>|
|<span data-ttu-id="fd449-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fd449-135">userEmailAddress</span></span>|<span data-ttu-id="fd449-136">String</span><span class="sxs-lookup"><span data-stu-id="fd449-136">String</span></span>|<span data-ttu-id="fd449-137">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="fd449-137">The user email address.</span></span>|
|<span data-ttu-id="fd449-138">userId</span><span class="sxs-lookup"><span data-stu-id="fd449-138">userId</span></span>|<span data-ttu-id="fd449-139">String</span><span class="sxs-lookup"><span data-stu-id="fd449-139">String</span></span>|<span data-ttu-id="fd449-140">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="fd449-140">The user ID.</span></span>|
|<span data-ttu-id="fd449-141">userName</span><span class="sxs-lookup"><span data-stu-id="fd449-141">userName</span></span>|<span data-ttu-id="fd449-142">String</span><span class="sxs-lookup"><span data-stu-id="fd449-142">String</span></span>|<span data-ttu-id="fd449-143">用户名。</span><span class="sxs-lookup"><span data-stu-id="fd449-143">The user name.</span></span>|
|<span data-ttu-id="fd449-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd449-144">userPrincipalName</span></span>|<span data-ttu-id="fd449-145">字符串</span><span class="sxs-lookup"><span data-stu-id="fd449-145">String</span></span>|<span data-ttu-id="fd449-146">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="fd449-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="fd449-147">响应</span><span class="sxs-lookup"><span data-stu-id="fd449-147">Response</span></span>
<span data-ttu-id="fd449-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd449-148">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd449-149">示例</span><span class="sxs-lookup"><span data-stu-id="fd449-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd449-150">请求</span><span class="sxs-lookup"><span data-stu-id="fd449-150">Request</span></span>
<span data-ttu-id="fd449-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd449-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fd449-152">响应</span><span class="sxs-lookup"><span data-stu-id="fd449-152">Response</span></span>
<span data-ttu-id="fd449-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd449-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




