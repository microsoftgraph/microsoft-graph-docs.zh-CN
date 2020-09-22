---
title: 创建 iosVppAppAssignedLicense
description: 创建新的 iosVppAppAssignedLicense 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b86d8e27adaac44dab2d18155d0f1ebfd18f2ed1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012227"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="66ac1-103">创建 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="66ac1-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="66ac1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ac1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66ac1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66ac1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66ac1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66ac1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66ac1-107">创建新的 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66ac1-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66ac1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="66ac1-108">Prerequisites</span></span>
<span data-ttu-id="66ac1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66ac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66ac1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="66ac1-111">Permission type</span></span>|<span data-ttu-id="66ac1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66ac1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66ac1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66ac1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66ac1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66ac1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66ac1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66ac1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66ac1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66ac1-116">Not supported.</span></span>|
|<span data-ttu-id="66ac1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="66ac1-117">Application</span></span>|<span data-ttu-id="66ac1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66ac1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66ac1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66ac1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="66ac1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66ac1-120">Request headers</span></span>
|<span data-ttu-id="66ac1-121">标头</span><span class="sxs-lookup"><span data-stu-id="66ac1-121">Header</span></span>|<span data-ttu-id="66ac1-122">值</span><span class="sxs-lookup"><span data-stu-id="66ac1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66ac1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66ac1-123">Authorization</span></span>|<span data-ttu-id="66ac1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66ac1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66ac1-125">接受</span><span class="sxs-lookup"><span data-stu-id="66ac1-125">Accept</span></span>|<span data-ttu-id="66ac1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66ac1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66ac1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66ac1-127">Request body</span></span>
<span data-ttu-id="66ac1-128">在请求正文中，提供 iosVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66ac1-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="66ac1-129">下表显示创建 iosVppAppAssignedLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66ac1-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="66ac1-130">属性</span><span class="sxs-lookup"><span data-stu-id="66ac1-130">Property</span></span>|<span data-ttu-id="66ac1-131">类型</span><span class="sxs-lookup"><span data-stu-id="66ac1-131">Type</span></span>|<span data-ttu-id="66ac1-132">说明</span><span class="sxs-lookup"><span data-stu-id="66ac1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66ac1-133">id</span><span class="sxs-lookup"><span data-stu-id="66ac1-133">id</span></span>|<span data-ttu-id="66ac1-134">String</span><span class="sxs-lookup"><span data-stu-id="66ac1-134">String</span></span>|<span data-ttu-id="66ac1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66ac1-135">Key of the entity.</span></span>|
|<span data-ttu-id="66ac1-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="66ac1-136">userEmailAddress</span></span>|<span data-ttu-id="66ac1-137">String</span><span class="sxs-lookup"><span data-stu-id="66ac1-137">String</span></span>|<span data-ttu-id="66ac1-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="66ac1-138">The user email address.</span></span>|
|<span data-ttu-id="66ac1-139">userId</span><span class="sxs-lookup"><span data-stu-id="66ac1-139">userId</span></span>|<span data-ttu-id="66ac1-140">String</span><span class="sxs-lookup"><span data-stu-id="66ac1-140">String</span></span>|<span data-ttu-id="66ac1-141">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="66ac1-141">The user ID.</span></span>|
|<span data-ttu-id="66ac1-142">userName</span><span class="sxs-lookup"><span data-stu-id="66ac1-142">userName</span></span>|<span data-ttu-id="66ac1-143">String</span><span class="sxs-lookup"><span data-stu-id="66ac1-143">String</span></span>|<span data-ttu-id="66ac1-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="66ac1-144">The user name.</span></span>|
|<span data-ttu-id="66ac1-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="66ac1-145">userPrincipalName</span></span>|<span data-ttu-id="66ac1-146">String</span><span class="sxs-lookup"><span data-stu-id="66ac1-146">String</span></span>|<span data-ttu-id="66ac1-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="66ac1-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="66ac1-148">响应</span><span class="sxs-lookup"><span data-stu-id="66ac1-148">Response</span></span>
<span data-ttu-id="66ac1-149">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66ac1-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66ac1-150">示例</span><span class="sxs-lookup"><span data-stu-id="66ac1-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="66ac1-151">请求</span><span class="sxs-lookup"><span data-stu-id="66ac1-151">Request</span></span>
<span data-ttu-id="66ac1-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66ac1-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66ac1-153">响应</span><span class="sxs-lookup"><span data-stu-id="66ac1-153">Response</span></span>
<span data-ttu-id="66ac1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66ac1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






