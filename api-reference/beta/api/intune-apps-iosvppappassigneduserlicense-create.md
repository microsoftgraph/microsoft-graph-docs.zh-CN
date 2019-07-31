---
title: 创建 iosVppAppAssignedUserLicense
description: 创建新的 iosVppAppAssignedUserLicense 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd0cdc0d54a7be9bad39fd75cf39e91c4d015cc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962293"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="a92cd-103">创建 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="a92cd-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="a92cd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a92cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a92cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a92cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a92cd-106">创建新的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a92cd-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a92cd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a92cd-107">Prerequisites</span></span>
<span data-ttu-id="a92cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a92cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a92cd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a92cd-110">Permission type</span></span>|<span data-ttu-id="a92cd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a92cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a92cd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a92cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a92cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a92cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a92cd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a92cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a92cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a92cd-115">Not supported.</span></span>|
|<span data-ttu-id="a92cd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a92cd-116">Application</span></span>|<span data-ttu-id="a92cd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a92cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a92cd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a92cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="a92cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a92cd-119">Request headers</span></span>
|<span data-ttu-id="a92cd-120">标头</span><span class="sxs-lookup"><span data-stu-id="a92cd-120">Header</span></span>|<span data-ttu-id="a92cd-121">值</span><span class="sxs-lookup"><span data-stu-id="a92cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a92cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a92cd-122">Authorization</span></span>|<span data-ttu-id="a92cd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a92cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a92cd-124">接受</span><span class="sxs-lookup"><span data-stu-id="a92cd-124">Accept</span></span>|<span data-ttu-id="a92cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a92cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a92cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a92cd-126">Request body</span></span>
<span data-ttu-id="a92cd-127">在请求正文中, 提供 iosVppAppAssignedUserLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a92cd-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="a92cd-128">下表显示创建 iosVppAppAssignedUserLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a92cd-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="a92cd-129">属性</span><span class="sxs-lookup"><span data-stu-id="a92cd-129">Property</span></span>|<span data-ttu-id="a92cd-130">类型</span><span class="sxs-lookup"><span data-stu-id="a92cd-130">Type</span></span>|<span data-ttu-id="a92cd-131">说明</span><span class="sxs-lookup"><span data-stu-id="a92cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a92cd-132">id</span><span class="sxs-lookup"><span data-stu-id="a92cd-132">id</span></span>|<span data-ttu-id="a92cd-133">String</span><span class="sxs-lookup"><span data-stu-id="a92cd-133">String</span></span>|<span data-ttu-id="a92cd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a92cd-134">Key of the entity.</span></span> <span data-ttu-id="a92cd-135">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a92cd-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a92cd-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a92cd-136">userEmailAddress</span></span>|<span data-ttu-id="a92cd-137">String</span><span class="sxs-lookup"><span data-stu-id="a92cd-137">String</span></span>|<span data-ttu-id="a92cd-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a92cd-138">The user email address.</span></span> <span data-ttu-id="a92cd-139">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a92cd-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a92cd-140">userId</span><span class="sxs-lookup"><span data-stu-id="a92cd-140">userId</span></span>|<span data-ttu-id="a92cd-141">String</span><span class="sxs-lookup"><span data-stu-id="a92cd-141">String</span></span>|<span data-ttu-id="a92cd-142">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="a92cd-142">The user ID.</span></span> <span data-ttu-id="a92cd-143">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a92cd-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a92cd-144">userName</span><span class="sxs-lookup"><span data-stu-id="a92cd-144">userName</span></span>|<span data-ttu-id="a92cd-145">String</span><span class="sxs-lookup"><span data-stu-id="a92cd-145">String</span></span>|<span data-ttu-id="a92cd-146">用户名。</span><span class="sxs-lookup"><span data-stu-id="a92cd-146">The user name.</span></span> <span data-ttu-id="a92cd-147">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a92cd-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a92cd-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a92cd-148">userPrincipalName</span></span>|<span data-ttu-id="a92cd-149">字符串</span><span class="sxs-lookup"><span data-stu-id="a92cd-149">String</span></span>|<span data-ttu-id="a92cd-150">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a92cd-150">The user principal name.</span></span> <span data-ttu-id="a92cd-151">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a92cd-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a92cd-152">响应</span><span class="sxs-lookup"><span data-stu-id="a92cd-152">Response</span></span>
<span data-ttu-id="a92cd-153">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a92cd-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a92cd-154">示例</span><span class="sxs-lookup"><span data-stu-id="a92cd-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a92cd-155">请求</span><span class="sxs-lookup"><span data-stu-id="a92cd-155">Request</span></span>
<span data-ttu-id="a92cd-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a92cd-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a92cd-157">响应</span><span class="sxs-lookup"><span data-stu-id="a92cd-157">Response</span></span>
<span data-ttu-id="a92cd-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a92cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





