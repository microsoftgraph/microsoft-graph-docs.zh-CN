---
title: 更新 iosVppAppAssignedLicense
description: 更新 iosVppAppAssignedLicense 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 430946a5202eab70bc0ffa24c502eba125d06e40
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700022"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="f1af2-103">更新 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="f1af2-103">Update iosVppAppAssignedLicense</span></span>

<span data-ttu-id="f1af2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1af2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1af2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1af2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1af2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1af2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1af2-107">更新 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1af2-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1af2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1af2-108">Prerequisites</span></span>
<span data-ttu-id="f1af2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1af2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1af2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1af2-111">Permission type</span></span>|<span data-ttu-id="f1af2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1af2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1af2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1af2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1af2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1af2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1af2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1af2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1af2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1af2-116">Not supported.</span></span>|
|<span data-ttu-id="f1af2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1af2-117">Application</span></span>|<span data-ttu-id="f1af2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1af2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1af2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1af2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f1af2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1af2-120">Request headers</span></span>
|<span data-ttu-id="f1af2-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1af2-121">Header</span></span>|<span data-ttu-id="f1af2-122">值</span><span class="sxs-lookup"><span data-stu-id="f1af2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1af2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1af2-123">Authorization</span></span>|<span data-ttu-id="f1af2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1af2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1af2-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1af2-125">Accept</span></span>|<span data-ttu-id="f1af2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1af2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1af2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1af2-127">Request body</span></span>
<span data-ttu-id="f1af2-128">在请求正文中，提供 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1af2-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="f1af2-129">下表显示创建 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1af2-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="f1af2-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1af2-130">Property</span></span>|<span data-ttu-id="f1af2-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1af2-131">Type</span></span>|<span data-ttu-id="f1af2-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1af2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1af2-133">id</span><span class="sxs-lookup"><span data-stu-id="f1af2-133">id</span></span>|<span data-ttu-id="f1af2-134">String</span><span class="sxs-lookup"><span data-stu-id="f1af2-134">String</span></span>|<span data-ttu-id="f1af2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1af2-135">Key of the entity.</span></span>|
|<span data-ttu-id="f1af2-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f1af2-136">userEmailAddress</span></span>|<span data-ttu-id="f1af2-137">String</span><span class="sxs-lookup"><span data-stu-id="f1af2-137">String</span></span>|<span data-ttu-id="f1af2-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f1af2-138">The user email address.</span></span>|
|<span data-ttu-id="f1af2-139">userId</span><span class="sxs-lookup"><span data-stu-id="f1af2-139">userId</span></span>|<span data-ttu-id="f1af2-140">String</span><span class="sxs-lookup"><span data-stu-id="f1af2-140">String</span></span>|<span data-ttu-id="f1af2-141">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="f1af2-141">The user ID.</span></span>|
|<span data-ttu-id="f1af2-142">userName</span><span class="sxs-lookup"><span data-stu-id="f1af2-142">userName</span></span>|<span data-ttu-id="f1af2-143">String</span><span class="sxs-lookup"><span data-stu-id="f1af2-143">String</span></span>|<span data-ttu-id="f1af2-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="f1af2-144">The user name.</span></span>|
|<span data-ttu-id="f1af2-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1af2-145">userPrincipalName</span></span>|<span data-ttu-id="f1af2-146">String</span><span class="sxs-lookup"><span data-stu-id="f1af2-146">String</span></span>|<span data-ttu-id="f1af2-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="f1af2-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="f1af2-148">响应</span><span class="sxs-lookup"><span data-stu-id="f1af2-148">Response</span></span>
<span data-ttu-id="f1af2-149">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1af2-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1af2-150">示例</span><span class="sxs-lookup"><span data-stu-id="f1af2-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1af2-151">请求</span><span class="sxs-lookup"><span data-stu-id="f1af2-151">Request</span></span>
<span data-ttu-id="f1af2-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1af2-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1af2-153">响应</span><span class="sxs-lookup"><span data-stu-id="f1af2-153">Response</span></span>
<span data-ttu-id="f1af2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1af2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





