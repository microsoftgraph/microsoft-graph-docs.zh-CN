---
title: 更新 iosVppAppAssignedUserLicense
description: 更新 iosVppAppAssignedUserLicense 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70ed9e2027a9ef5f8b87fea2e7bd06e2e8ac6e67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445426"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="2a234-103">更新 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="2a234-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="2a234-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2a234-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a234-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a234-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a234-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a234-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a234-107">更新[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a234-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a234-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a234-108">Prerequisites</span></span>
<span data-ttu-id="2a234-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a234-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a234-111">Permission type</span></span>|<span data-ttu-id="2a234-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a234-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a234-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a234-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a234-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a234-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a234-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a234-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a234-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a234-116">Not supported.</span></span>|
|<span data-ttu-id="2a234-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a234-117">Application</span></span>|<span data-ttu-id="2a234-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a234-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a234-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a234-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="2a234-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a234-120">Request headers</span></span>
|<span data-ttu-id="2a234-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a234-121">Header</span></span>|<span data-ttu-id="2a234-122">值</span><span class="sxs-lookup"><span data-stu-id="2a234-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a234-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a234-123">Authorization</span></span>|<span data-ttu-id="2a234-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a234-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a234-125">接受</span><span class="sxs-lookup"><span data-stu-id="2a234-125">Accept</span></span>|<span data-ttu-id="2a234-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a234-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a234-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a234-127">Request body</span></span>
<span data-ttu-id="2a234-128">在请求正文中，提供[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a234-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="2a234-129">下表显示创建[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a234-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="2a234-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a234-130">Property</span></span>|<span data-ttu-id="2a234-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a234-131">Type</span></span>|<span data-ttu-id="2a234-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a234-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a234-133">id</span><span class="sxs-lookup"><span data-stu-id="2a234-133">id</span></span>|<span data-ttu-id="2a234-134">String</span><span class="sxs-lookup"><span data-stu-id="2a234-134">String</span></span>|<span data-ttu-id="2a234-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a234-135">Key of the entity.</span></span> <span data-ttu-id="2a234-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2a234-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2a234-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2a234-137">userEmailAddress</span></span>|<span data-ttu-id="2a234-138">String</span><span class="sxs-lookup"><span data-stu-id="2a234-138">String</span></span>|<span data-ttu-id="2a234-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2a234-139">The user email address.</span></span> <span data-ttu-id="2a234-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2a234-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2a234-141">userId</span><span class="sxs-lookup"><span data-stu-id="2a234-141">userId</span></span>|<span data-ttu-id="2a234-142">String</span><span class="sxs-lookup"><span data-stu-id="2a234-142">String</span></span>|<span data-ttu-id="2a234-143">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2a234-143">The user ID.</span></span> <span data-ttu-id="2a234-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2a234-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2a234-145">userName</span><span class="sxs-lookup"><span data-stu-id="2a234-145">userName</span></span>|<span data-ttu-id="2a234-146">String</span><span class="sxs-lookup"><span data-stu-id="2a234-146">String</span></span>|<span data-ttu-id="2a234-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="2a234-147">The user name.</span></span> <span data-ttu-id="2a234-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2a234-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2a234-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a234-149">userPrincipalName</span></span>|<span data-ttu-id="2a234-150">字符串</span><span class="sxs-lookup"><span data-stu-id="2a234-150">String</span></span>|<span data-ttu-id="2a234-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="2a234-151">The user principal name.</span></span> <span data-ttu-id="2a234-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2a234-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2a234-153">响应</span><span class="sxs-lookup"><span data-stu-id="2a234-153">Response</span></span>
<span data-ttu-id="2a234-154">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a234-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a234-155">示例</span><span class="sxs-lookup"><span data-stu-id="2a234-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a234-156">请求</span><span class="sxs-lookup"><span data-stu-id="2a234-156">Request</span></span>
<span data-ttu-id="2a234-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a234-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a234-158">响应</span><span class="sxs-lookup"><span data-stu-id="2a234-158">Response</span></span>
<span data-ttu-id="2a234-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a234-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





