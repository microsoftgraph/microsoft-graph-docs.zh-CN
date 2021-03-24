---
title: 更新 iosVppAppAssignedUserLicense
description: 更新 iosVppAppAssignedUserLicense 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a257dd6f866ae58e7eafd12f36320d7c7f7baf4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140537"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="65b39-103">更新 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="65b39-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="65b39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65b39-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65b39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65b39-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65b39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65b39-107">更新 [iosVppAppAssignedUserLicense 对象](../resources/intune-apps-iosvppappassigneduserlicense.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="65b39-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65b39-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="65b39-108">Prerequisites</span></span>
<span data-ttu-id="65b39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65b39-111">Permission type</span></span>|<span data-ttu-id="65b39-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65b39-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65b39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65b39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65b39-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b39-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65b39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65b39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65b39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65b39-116">Not supported.</span></span>|
|<span data-ttu-id="65b39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65b39-117">Application</span></span>|<span data-ttu-id="65b39-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b39-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65b39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65b39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="65b39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65b39-120">Request headers</span></span>
|<span data-ttu-id="65b39-121">标头</span><span class="sxs-lookup"><span data-stu-id="65b39-121">Header</span></span>|<span data-ttu-id="65b39-122">值</span><span class="sxs-lookup"><span data-stu-id="65b39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65b39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b39-123">Authorization</span></span>|<span data-ttu-id="65b39-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65b39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65b39-125">接受</span><span class="sxs-lookup"><span data-stu-id="65b39-125">Accept</span></span>|<span data-ttu-id="65b39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65b39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65b39-127">Request body</span></span>
<span data-ttu-id="65b39-128">在请求正文中，提供 [iosVppAppAssignedUserLicense 对象的](../resources/intune-apps-iosvppappassigneduserlicense.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65b39-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="65b39-129">下表显示创建 [iosVppAppAssignedUserLicense 时所需的属性](../resources/intune-apps-iosvppappassigneduserlicense.md)。</span><span class="sxs-lookup"><span data-stu-id="65b39-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="65b39-130">属性</span><span class="sxs-lookup"><span data-stu-id="65b39-130">Property</span></span>|<span data-ttu-id="65b39-131">类型</span><span class="sxs-lookup"><span data-stu-id="65b39-131">Type</span></span>|<span data-ttu-id="65b39-132">说明</span><span class="sxs-lookup"><span data-stu-id="65b39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b39-133">id</span><span class="sxs-lookup"><span data-stu-id="65b39-133">id</span></span>|<span data-ttu-id="65b39-134">String</span><span class="sxs-lookup"><span data-stu-id="65b39-134">String</span></span>|<span data-ttu-id="65b39-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65b39-135">Key of the entity.</span></span> <span data-ttu-id="65b39-136">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="65b39-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="65b39-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="65b39-137">userEmailAddress</span></span>|<span data-ttu-id="65b39-138">String</span><span class="sxs-lookup"><span data-stu-id="65b39-138">String</span></span>|<span data-ttu-id="65b39-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="65b39-139">The user email address.</span></span> <span data-ttu-id="65b39-140">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="65b39-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="65b39-141">userId</span><span class="sxs-lookup"><span data-stu-id="65b39-141">userId</span></span>|<span data-ttu-id="65b39-142">String</span><span class="sxs-lookup"><span data-stu-id="65b39-142">String</span></span>|<span data-ttu-id="65b39-143">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="65b39-143">The user ID.</span></span> <span data-ttu-id="65b39-144">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="65b39-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="65b39-145">userName</span><span class="sxs-lookup"><span data-stu-id="65b39-145">userName</span></span>|<span data-ttu-id="65b39-146">String</span><span class="sxs-lookup"><span data-stu-id="65b39-146">String</span></span>|<span data-ttu-id="65b39-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="65b39-147">The user name.</span></span> <span data-ttu-id="65b39-148">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="65b39-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="65b39-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65b39-149">userPrincipalName</span></span>|<span data-ttu-id="65b39-150">String</span><span class="sxs-lookup"><span data-stu-id="65b39-150">String</span></span>|<span data-ttu-id="65b39-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="65b39-151">The user principal name.</span></span> <span data-ttu-id="65b39-152">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="65b39-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="65b39-153">响应</span><span class="sxs-lookup"><span data-stu-id="65b39-153">Response</span></span>
<span data-ttu-id="65b39-154">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65b39-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65b39-155">示例</span><span class="sxs-lookup"><span data-stu-id="65b39-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="65b39-156">请求</span><span class="sxs-lookup"><span data-stu-id="65b39-156">Request</span></span>
<span data-ttu-id="65b39-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65b39-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65b39-158">响应</span><span class="sxs-lookup"><span data-stu-id="65b39-158">Response</span></span>
<span data-ttu-id="65b39-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65b39-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




