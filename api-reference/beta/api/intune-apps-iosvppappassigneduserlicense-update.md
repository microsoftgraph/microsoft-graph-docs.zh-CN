---
title: 更新 iosVppAppAssignedUserLicense
description: 更新 iosVppAppAssignedUserLicense 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e858e4ac9e473816ba0e7e3d08db08e60657ace2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761837"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="8c813-103">更新 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="8c813-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="8c813-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c813-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c813-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c813-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c813-106">更新[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c813-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c813-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c813-107">Prerequisites</span></span>
<span data-ttu-id="8c813-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c813-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c813-110">Permission type</span></span>|<span data-ttu-id="8c813-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c813-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c813-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c813-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c813-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c813-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c813-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c813-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c813-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c813-115">Not supported.</span></span>|
|<span data-ttu-id="8c813-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c813-116">Application</span></span>|<span data-ttu-id="8c813-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c813-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c813-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c813-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="8c813-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c813-119">Request headers</span></span>
|<span data-ttu-id="8c813-120">标头</span><span class="sxs-lookup"><span data-stu-id="8c813-120">Header</span></span>|<span data-ttu-id="8c813-121">值</span><span class="sxs-lookup"><span data-stu-id="8c813-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c813-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c813-122">Authorization</span></span>|<span data-ttu-id="8c813-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c813-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c813-124">接受</span><span class="sxs-lookup"><span data-stu-id="8c813-124">Accept</span></span>|<span data-ttu-id="8c813-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c813-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c813-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c813-126">Request body</span></span>
<span data-ttu-id="8c813-127">在请求正文中，提供[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c813-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="8c813-128">下表显示创建[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c813-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="8c813-129">属性</span><span class="sxs-lookup"><span data-stu-id="8c813-129">Property</span></span>|<span data-ttu-id="8c813-130">类型</span><span class="sxs-lookup"><span data-stu-id="8c813-130">Type</span></span>|<span data-ttu-id="8c813-131">说明</span><span class="sxs-lookup"><span data-stu-id="8c813-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c813-132">id</span><span class="sxs-lookup"><span data-stu-id="8c813-132">id</span></span>|<span data-ttu-id="8c813-133">String</span><span class="sxs-lookup"><span data-stu-id="8c813-133">String</span></span>|<span data-ttu-id="8c813-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8c813-134">Key of the entity.</span></span> <span data-ttu-id="8c813-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8c813-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8c813-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8c813-136">userEmailAddress</span></span>|<span data-ttu-id="8c813-137">String</span><span class="sxs-lookup"><span data-stu-id="8c813-137">String</span></span>|<span data-ttu-id="8c813-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8c813-138">The user email address.</span></span> <span data-ttu-id="8c813-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8c813-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8c813-140">userId</span><span class="sxs-lookup"><span data-stu-id="8c813-140">userId</span></span>|<span data-ttu-id="8c813-141">String</span><span class="sxs-lookup"><span data-stu-id="8c813-141">String</span></span>|<span data-ttu-id="8c813-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8c813-142">The user ID.</span></span> <span data-ttu-id="8c813-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8c813-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8c813-144">userName</span><span class="sxs-lookup"><span data-stu-id="8c813-144">userName</span></span>|<span data-ttu-id="8c813-145">String</span><span class="sxs-lookup"><span data-stu-id="8c813-145">String</span></span>|<span data-ttu-id="8c813-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="8c813-146">The user name.</span></span> <span data-ttu-id="8c813-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8c813-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8c813-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c813-148">userPrincipalName</span></span>|<span data-ttu-id="8c813-149">字符串</span><span class="sxs-lookup"><span data-stu-id="8c813-149">String</span></span>|<span data-ttu-id="8c813-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="8c813-150">The user principal name.</span></span> <span data-ttu-id="8c813-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8c813-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8c813-152">响应</span><span class="sxs-lookup"><span data-stu-id="8c813-152">Response</span></span>
<span data-ttu-id="8c813-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c813-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c813-154">示例</span><span class="sxs-lookup"><span data-stu-id="8c813-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c813-155">请求</span><span class="sxs-lookup"><span data-stu-id="8c813-155">Request</span></span>
<span data-ttu-id="8c813-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c813-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8c813-157">响应</span><span class="sxs-lookup"><span data-stu-id="8c813-157">Response</span></span>
<span data-ttu-id="8c813-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c813-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




