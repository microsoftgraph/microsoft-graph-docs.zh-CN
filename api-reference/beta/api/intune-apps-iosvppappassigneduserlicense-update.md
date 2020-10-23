---
title: 更新 iosVppAppAssignedUserLicense
description: 更新 iosVppAppAssignedUserLicense 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7e42fab59d46118ab5c32223934add18d415bd0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699987"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="4dd3b-103">更新 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="4dd3b-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="4dd3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dd3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dd3b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dd3b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dd3b-107">更新 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dd3b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4dd3b-108">Prerequisites</span></span>
<span data-ttu-id="4dd3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dd3b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dd3b-111">Permission type</span></span>|<span data-ttu-id="4dd3b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4dd3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dd3b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4dd3b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd3b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4dd3b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dd3b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-116">Not supported.</span></span>|
|<span data-ttu-id="4dd3b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dd3b-117">Application</span></span>|<span data-ttu-id="4dd3b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd3b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dd3b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dd3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="4dd3b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dd3b-120">Request headers</span></span>
|<span data-ttu-id="4dd3b-121">标头</span><span class="sxs-lookup"><span data-stu-id="4dd3b-121">Header</span></span>|<span data-ttu-id="4dd3b-122">值</span><span class="sxs-lookup"><span data-stu-id="4dd3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dd3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dd3b-123">Authorization</span></span>|<span data-ttu-id="4dd3b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dd3b-125">接受</span><span class="sxs-lookup"><span data-stu-id="4dd3b-125">Accept</span></span>|<span data-ttu-id="4dd3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4dd3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dd3b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dd3b-127">Request body</span></span>
<span data-ttu-id="4dd3b-128">在请求正文中，提供 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="4dd3b-129">下表显示创建 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="4dd3b-130">属性</span><span class="sxs-lookup"><span data-stu-id="4dd3b-130">Property</span></span>|<span data-ttu-id="4dd3b-131">类型</span><span class="sxs-lookup"><span data-stu-id="4dd3b-131">Type</span></span>|<span data-ttu-id="4dd3b-132">说明</span><span class="sxs-lookup"><span data-stu-id="4dd3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dd3b-133">id</span><span class="sxs-lookup"><span data-stu-id="4dd3b-133">id</span></span>|<span data-ttu-id="4dd3b-134">String</span><span class="sxs-lookup"><span data-stu-id="4dd3b-134">String</span></span>|<span data-ttu-id="4dd3b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-135">Key of the entity.</span></span> <span data-ttu-id="4dd3b-136">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4dd3b-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4dd3b-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4dd3b-137">userEmailAddress</span></span>|<span data-ttu-id="4dd3b-138">String</span><span class="sxs-lookup"><span data-stu-id="4dd3b-138">String</span></span>|<span data-ttu-id="4dd3b-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-139">The user email address.</span></span> <span data-ttu-id="4dd3b-140">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4dd3b-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4dd3b-141">userId</span><span class="sxs-lookup"><span data-stu-id="4dd3b-141">userId</span></span>|<span data-ttu-id="4dd3b-142">String</span><span class="sxs-lookup"><span data-stu-id="4dd3b-142">String</span></span>|<span data-ttu-id="4dd3b-143">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-143">The user ID.</span></span> <span data-ttu-id="4dd3b-144">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4dd3b-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4dd3b-145">userName</span><span class="sxs-lookup"><span data-stu-id="4dd3b-145">userName</span></span>|<span data-ttu-id="4dd3b-146">String</span><span class="sxs-lookup"><span data-stu-id="4dd3b-146">String</span></span>|<span data-ttu-id="4dd3b-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-147">The user name.</span></span> <span data-ttu-id="4dd3b-148">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4dd3b-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4dd3b-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4dd3b-149">userPrincipalName</span></span>|<span data-ttu-id="4dd3b-150">String</span><span class="sxs-lookup"><span data-stu-id="4dd3b-150">String</span></span>|<span data-ttu-id="4dd3b-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-151">The user principal name.</span></span> <span data-ttu-id="4dd3b-152">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4dd3b-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4dd3b-153">响应</span><span class="sxs-lookup"><span data-stu-id="4dd3b-153">Response</span></span>
<span data-ttu-id="4dd3b-154">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dd3b-155">示例</span><span class="sxs-lookup"><span data-stu-id="4dd3b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dd3b-156">请求</span><span class="sxs-lookup"><span data-stu-id="4dd3b-156">Request</span></span>
<span data-ttu-id="4dd3b-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4dd3b-158">响应</span><span class="sxs-lookup"><span data-stu-id="4dd3b-158">Response</span></span>
<span data-ttu-id="4dd3b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dd3b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





