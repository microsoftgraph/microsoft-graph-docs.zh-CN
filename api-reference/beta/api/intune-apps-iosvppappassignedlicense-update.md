---
title: 更新 iosVppAppAssignedLicense
description: 更新 iosVppAppAssignedLicense 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3946ee39c8be93a7c0323da868a65f76d54fc3c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397545"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="e59db-103">更新 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="e59db-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="e59db-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e59db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e59db-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e59db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e59db-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e59db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e59db-107">更新[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e59db-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e59db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e59db-108">Prerequisites</span></span>
<span data-ttu-id="e59db-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e59db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e59db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e59db-111">Permission type</span></span>|<span data-ttu-id="e59db-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e59db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e59db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e59db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e59db-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59db-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e59db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e59db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e59db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e59db-116">Not supported.</span></span>|
|<span data-ttu-id="e59db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e59db-117">Application</span></span>|<span data-ttu-id="e59db-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e59db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e59db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e59db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="e59db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e59db-120">Request headers</span></span>
|<span data-ttu-id="e59db-121">标头</span><span class="sxs-lookup"><span data-stu-id="e59db-121">Header</span></span>|<span data-ttu-id="e59db-122">值</span><span class="sxs-lookup"><span data-stu-id="e59db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e59db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e59db-123">Authorization</span></span>|<span data-ttu-id="e59db-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e59db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e59db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e59db-125">Accept</span></span>|<span data-ttu-id="e59db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e59db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e59db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e59db-127">Request body</span></span>
<span data-ttu-id="e59db-128">在请求正文中，提供[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e59db-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="e59db-129">下表显示时创建[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e59db-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="e59db-130">属性</span><span class="sxs-lookup"><span data-stu-id="e59db-130">Property</span></span>|<span data-ttu-id="e59db-131">类型</span><span class="sxs-lookup"><span data-stu-id="e59db-131">Type</span></span>|<span data-ttu-id="e59db-132">说明</span><span class="sxs-lookup"><span data-stu-id="e59db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59db-133">id</span><span class="sxs-lookup"><span data-stu-id="e59db-133">id</span></span>|<span data-ttu-id="e59db-134">String</span><span class="sxs-lookup"><span data-stu-id="e59db-134">String</span></span>|<span data-ttu-id="e59db-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e59db-135">Key of the entity.</span></span>|
|<span data-ttu-id="e59db-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e59db-136">userEmailAddress</span></span>|<span data-ttu-id="e59db-137">String</span><span class="sxs-lookup"><span data-stu-id="e59db-137">String</span></span>|<span data-ttu-id="e59db-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e59db-138">The user email address.</span></span>|
|<span data-ttu-id="e59db-139">userId</span><span class="sxs-lookup"><span data-stu-id="e59db-139">userId</span></span>|<span data-ttu-id="e59db-140">String</span><span class="sxs-lookup"><span data-stu-id="e59db-140">String</span></span>|<span data-ttu-id="e59db-141">用户 id。</span><span class="sxs-lookup"><span data-stu-id="e59db-141">The user ID.</span></span>|
|<span data-ttu-id="e59db-142">userName</span><span class="sxs-lookup"><span data-stu-id="e59db-142">userName</span></span>|<span data-ttu-id="e59db-143">String</span><span class="sxs-lookup"><span data-stu-id="e59db-143">String</span></span>|<span data-ttu-id="e59db-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="e59db-144">The user name.</span></span>|
|<span data-ttu-id="e59db-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e59db-145">userPrincipalName</span></span>|<span data-ttu-id="e59db-146">String</span><span class="sxs-lookup"><span data-stu-id="e59db-146">String</span></span>|<span data-ttu-id="e59db-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e59db-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="e59db-148">响应</span><span class="sxs-lookup"><span data-stu-id="e59db-148">Response</span></span>
<span data-ttu-id="e59db-149">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e59db-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e59db-150">示例</span><span class="sxs-lookup"><span data-stu-id="e59db-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e59db-151">请求</span><span class="sxs-lookup"><span data-stu-id="e59db-151">Request</span></span>
<span data-ttu-id="e59db-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e59db-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e59db-153">响应</span><span class="sxs-lookup"><span data-stu-id="e59db-153">Response</span></span>
<span data-ttu-id="e59db-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e59db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




