---
title: 创建 iosVppAppAssignedLicense
description: 创建新的 iosVppAppAssignedLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59d40d358809214c4ad04996c42f24cd4c97e634
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798927"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="7ec1a-103">创建 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="7ec1a-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="7ec1a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ec1a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ec1a-106">创建新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-106">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ec1a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ec1a-107">Prerequisites</span></span>
<span data-ttu-id="7ec1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ec1a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ec1a-110">Permission type</span></span>|<span data-ttu-id="7ec1a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ec1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ec1a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ec1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ec1a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ec1a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ec1a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ec1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ec1a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-115">Not supported.</span></span>|
|<span data-ttu-id="7ec1a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ec1a-116">Application</span></span>|<span data-ttu-id="7ec1a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ec1a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ec1a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="7ec1a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ec1a-119">Request headers</span></span>
|<span data-ttu-id="7ec1a-120">标头</span><span class="sxs-lookup"><span data-stu-id="7ec1a-120">Header</span></span>|<span data-ttu-id="7ec1a-121">值</span><span class="sxs-lookup"><span data-stu-id="7ec1a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ec1a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ec1a-122">Authorization</span></span>|<span data-ttu-id="7ec1a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ec1a-124">接受</span><span class="sxs-lookup"><span data-stu-id="7ec1a-124">Accept</span></span>|<span data-ttu-id="7ec1a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ec1a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ec1a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ec1a-126">Request body</span></span>
<span data-ttu-id="7ec1a-127">在请求正文中, 提供 iosVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-127">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="7ec1a-128">下表显示创建 iosVppAppAssignedLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-128">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="7ec1a-129">属性</span><span class="sxs-lookup"><span data-stu-id="7ec1a-129">Property</span></span>|<span data-ttu-id="7ec1a-130">类型</span><span class="sxs-lookup"><span data-stu-id="7ec1a-130">Type</span></span>|<span data-ttu-id="7ec1a-131">说明</span><span class="sxs-lookup"><span data-stu-id="7ec1a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ec1a-132">id</span><span class="sxs-lookup"><span data-stu-id="7ec1a-132">id</span></span>|<span data-ttu-id="7ec1a-133">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-133">String</span></span>|<span data-ttu-id="7ec1a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-134">Key of the entity.</span></span>|
|<span data-ttu-id="7ec1a-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7ec1a-135">userEmailAddress</span></span>|<span data-ttu-id="7ec1a-136">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-136">String</span></span>|<span data-ttu-id="7ec1a-137">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-137">The user email address.</span></span>|
|<span data-ttu-id="7ec1a-138">userId</span><span class="sxs-lookup"><span data-stu-id="7ec1a-138">userId</span></span>|<span data-ttu-id="7ec1a-139">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-139">String</span></span>|<span data-ttu-id="7ec1a-140">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-140">The user ID.</span></span>|
|<span data-ttu-id="7ec1a-141">userName</span><span class="sxs-lookup"><span data-stu-id="7ec1a-141">userName</span></span>|<span data-ttu-id="7ec1a-142">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-142">String</span></span>|<span data-ttu-id="7ec1a-143">用户名。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-143">The user name.</span></span>|
|<span data-ttu-id="7ec1a-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ec1a-144">userPrincipalName</span></span>|<span data-ttu-id="7ec1a-145">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-145">String</span></span>|<span data-ttu-id="7ec1a-146">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="7ec1a-147">响应</span><span class="sxs-lookup"><span data-stu-id="7ec1a-147">Response</span></span>
<span data-ttu-id="7ec1a-148">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-148">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ec1a-149">示例</span><span class="sxs-lookup"><span data-stu-id="7ec1a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ec1a-150">请求</span><span class="sxs-lookup"><span data-stu-id="7ec1a-150">Request</span></span>
<span data-ttu-id="7ec1a-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ec1a-152">响应</span><span class="sxs-lookup"><span data-stu-id="7ec1a-152">Response</span></span>
<span data-ttu-id="7ec1a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ec1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





