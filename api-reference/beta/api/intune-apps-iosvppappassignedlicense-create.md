---
title: 创建 iosVppAppAssignedLicense
description: 创建新的 iosVppAppAssignedLicense 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73a25e6f217f287811be7ce7b3a459c36727f1dc
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173484"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="65e97-103">创建 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="65e97-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="65e97-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65e97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65e97-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65e97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e97-106">创建新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65e97-106">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65e97-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="65e97-107">Prerequisites</span></span>
<span data-ttu-id="65e97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="65e97-110">Permission type</span></span>|<span data-ttu-id="65e97-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65e97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65e97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65e97-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e97-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65e97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65e97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65e97-115">Not supported.</span></span>|
|<span data-ttu-id="65e97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65e97-116">Application</span></span>|<span data-ttu-id="65e97-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e97-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e97-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65e97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="65e97-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65e97-119">Request headers</span></span>
|<span data-ttu-id="65e97-120">标头</span><span class="sxs-lookup"><span data-stu-id="65e97-120">Header</span></span>|<span data-ttu-id="65e97-121">值</span><span class="sxs-lookup"><span data-stu-id="65e97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65e97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e97-122">Authorization</span></span>|<span data-ttu-id="65e97-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65e97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65e97-124">接受</span><span class="sxs-lookup"><span data-stu-id="65e97-124">Accept</span></span>|<span data-ttu-id="65e97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65e97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65e97-126">Request body</span></span>
<span data-ttu-id="65e97-127">在请求正文中，提供 iosVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65e97-127">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="65e97-128">下表显示创建 iosVppAppAssignedLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65e97-128">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="65e97-129">属性</span><span class="sxs-lookup"><span data-stu-id="65e97-129">Property</span></span>|<span data-ttu-id="65e97-130">类型</span><span class="sxs-lookup"><span data-stu-id="65e97-130">Type</span></span>|<span data-ttu-id="65e97-131">说明</span><span class="sxs-lookup"><span data-stu-id="65e97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e97-132">id</span><span class="sxs-lookup"><span data-stu-id="65e97-132">id</span></span>|<span data-ttu-id="65e97-133">String</span><span class="sxs-lookup"><span data-stu-id="65e97-133">String</span></span>|<span data-ttu-id="65e97-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65e97-134">Key of the entity.</span></span>|
|<span data-ttu-id="65e97-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="65e97-135">userEmailAddress</span></span>|<span data-ttu-id="65e97-136">String</span><span class="sxs-lookup"><span data-stu-id="65e97-136">String</span></span>|<span data-ttu-id="65e97-137">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="65e97-137">The user email address.</span></span>|
|<span data-ttu-id="65e97-138">userId</span><span class="sxs-lookup"><span data-stu-id="65e97-138">userId</span></span>|<span data-ttu-id="65e97-139">String</span><span class="sxs-lookup"><span data-stu-id="65e97-139">String</span></span>|<span data-ttu-id="65e97-140">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="65e97-140">The user ID.</span></span>|
|<span data-ttu-id="65e97-141">userName</span><span class="sxs-lookup"><span data-stu-id="65e97-141">userName</span></span>|<span data-ttu-id="65e97-142">String</span><span class="sxs-lookup"><span data-stu-id="65e97-142">String</span></span>|<span data-ttu-id="65e97-143">用户名。</span><span class="sxs-lookup"><span data-stu-id="65e97-143">The user name.</span></span>|
|<span data-ttu-id="65e97-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65e97-144">userPrincipalName</span></span>|<span data-ttu-id="65e97-145">字符串</span><span class="sxs-lookup"><span data-stu-id="65e97-145">String</span></span>|<span data-ttu-id="65e97-146">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="65e97-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="65e97-147">响应</span><span class="sxs-lookup"><span data-stu-id="65e97-147">Response</span></span>
<span data-ttu-id="65e97-148">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="65e97-148">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65e97-149">示例</span><span class="sxs-lookup"><span data-stu-id="65e97-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="65e97-150">请求</span><span class="sxs-lookup"><span data-stu-id="65e97-150">Request</span></span>
<span data-ttu-id="65e97-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65e97-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="65e97-152">响应</span><span class="sxs-lookup"><span data-stu-id="65e97-152">Response</span></span>
<span data-ttu-id="65e97-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65e97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




