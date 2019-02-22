---
title: 创建 iosVppAppAssignedUserLicense
description: 创建新的 iosVppAppAssignedUserLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f1efba3659190080c507ca3418bacd9bc7d6461
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157524"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="11504-103">创建 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="11504-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="11504-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11504-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11504-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11504-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11504-106">创建新的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11504-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11504-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="11504-107">Prerequisites</span></span>
<span data-ttu-id="11504-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="11504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="11504-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11504-110">Permission type</span></span>|<span data-ttu-id="11504-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11504-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11504-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11504-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11504-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11504-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11504-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11504-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11504-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11504-115">Not supported.</span></span>|
|<span data-ttu-id="11504-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11504-116">Application</span></span>|<span data-ttu-id="11504-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="11504-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11504-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11504-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="11504-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="11504-119">Request headers</span></span>
|<span data-ttu-id="11504-120">标头</span><span class="sxs-lookup"><span data-stu-id="11504-120">Header</span></span>|<span data-ttu-id="11504-121">值</span><span class="sxs-lookup"><span data-stu-id="11504-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11504-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11504-122">Authorization</span></span>|<span data-ttu-id="11504-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="11504-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11504-124">Accept</span><span class="sxs-lookup"><span data-stu-id="11504-124">Accept</span></span>|<span data-ttu-id="11504-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11504-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11504-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="11504-126">Request body</span></span>
<span data-ttu-id="11504-127">在请求正文中, 提供 iosVppAppAssignedUserLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11504-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="11504-128">下表显示创建 iosVppAppAssignedUserLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="11504-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="11504-129">属性</span><span class="sxs-lookup"><span data-stu-id="11504-129">Property</span></span>|<span data-ttu-id="11504-130">类型</span><span class="sxs-lookup"><span data-stu-id="11504-130">Type</span></span>|<span data-ttu-id="11504-131">说明</span><span class="sxs-lookup"><span data-stu-id="11504-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11504-132">id</span><span class="sxs-lookup"><span data-stu-id="11504-132">id</span></span>|<span data-ttu-id="11504-133">String</span><span class="sxs-lookup"><span data-stu-id="11504-133">String</span></span>|<span data-ttu-id="11504-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="11504-134">Key of the entity.</span></span> <span data-ttu-id="11504-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="11504-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="11504-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="11504-136">userEmailAddress</span></span>|<span data-ttu-id="11504-137">字符串</span><span class="sxs-lookup"><span data-stu-id="11504-137">String</span></span>|<span data-ttu-id="11504-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="11504-138">The user email address.</span></span> <span data-ttu-id="11504-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="11504-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="11504-140">userId</span><span class="sxs-lookup"><span data-stu-id="11504-140">userId</span></span>|<span data-ttu-id="11504-141">String</span><span class="sxs-lookup"><span data-stu-id="11504-141">String</span></span>|<span data-ttu-id="11504-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="11504-142">The user ID.</span></span> <span data-ttu-id="11504-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="11504-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="11504-144">userName</span><span class="sxs-lookup"><span data-stu-id="11504-144">userName</span></span>|<span data-ttu-id="11504-145">String</span><span class="sxs-lookup"><span data-stu-id="11504-145">String</span></span>|<span data-ttu-id="11504-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="11504-146">The user name.</span></span> <span data-ttu-id="11504-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="11504-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="11504-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="11504-148">userPrincipalName</span></span>|<span data-ttu-id="11504-149">字符串</span><span class="sxs-lookup"><span data-stu-id="11504-149">String</span></span>|<span data-ttu-id="11504-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="11504-150">The user principal name.</span></span> <span data-ttu-id="11504-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="11504-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="11504-152">响应</span><span class="sxs-lookup"><span data-stu-id="11504-152">Response</span></span>
<span data-ttu-id="11504-153">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11504-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11504-154">示例</span><span class="sxs-lookup"><span data-stu-id="11504-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="11504-155">请求</span><span class="sxs-lookup"><span data-stu-id="11504-155">Request</span></span>
<span data-ttu-id="11504-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11504-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="11504-157">响应</span><span class="sxs-lookup"><span data-stu-id="11504-157">Response</span></span>
<span data-ttu-id="11504-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="11504-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




