---
title: 创建 iosVppAppAssignedUserLicense
description: 创建新的 iosVppAppAssignedUserLicense 对象。
author: tfitzmac
ms.openlocfilehash: 93b92d28a73e253eb598d03d3171318d95d3fd8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308979"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="699f6-103">创建 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="699f6-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="699f6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="699f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="699f6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="699f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="699f6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="699f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="699f6-107">创建新的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="699f6-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="699f6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="699f6-108">Prerequisites</span></span>
<span data-ttu-id="699f6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="699f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="699f6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="699f6-111">Permission type</span></span>|<span data-ttu-id="699f6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="699f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="699f6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="699f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="699f6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="699f6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="699f6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="699f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="699f6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="699f6-116">Not supported.</span></span>|
|<span data-ttu-id="699f6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="699f6-117">Application</span></span>|<span data-ttu-id="699f6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="699f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="699f6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="699f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="699f6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="699f6-120">Request headers</span></span>
|<span data-ttu-id="699f6-121">标头</span><span class="sxs-lookup"><span data-stu-id="699f6-121">Header</span></span>|<span data-ttu-id="699f6-122">值</span><span class="sxs-lookup"><span data-stu-id="699f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="699f6-123">授权</span><span class="sxs-lookup"><span data-stu-id="699f6-123">Authorization</span></span>|<span data-ttu-id="699f6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="699f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="699f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="699f6-125">Accept</span></span>|<span data-ttu-id="699f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="699f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="699f6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="699f6-127">Request body</span></span>
<span data-ttu-id="699f6-128">在请求正文中，提供 iosVppAppAssignedUserLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="699f6-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="699f6-129">下表显示时创建 iosVppAppAssignedUserLicense 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="699f6-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="699f6-130">属性</span><span class="sxs-lookup"><span data-stu-id="699f6-130">Property</span></span>|<span data-ttu-id="699f6-131">类型</span><span class="sxs-lookup"><span data-stu-id="699f6-131">Type</span></span>|<span data-ttu-id="699f6-132">说明</span><span class="sxs-lookup"><span data-stu-id="699f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="699f6-133">id</span><span class="sxs-lookup"><span data-stu-id="699f6-133">id</span></span>|<span data-ttu-id="699f6-134">String</span><span class="sxs-lookup"><span data-stu-id="699f6-134">String</span></span>|<span data-ttu-id="699f6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="699f6-135">Key of the entity.</span></span> <span data-ttu-id="699f6-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="699f6-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="699f6-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="699f6-137">userEmailAddress</span></span>|<span data-ttu-id="699f6-138">字符串</span><span class="sxs-lookup"><span data-stu-id="699f6-138">String</span></span>|<span data-ttu-id="699f6-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="699f6-139">The user email address.</span></span> <span data-ttu-id="699f6-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="699f6-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="699f6-141">userId</span><span class="sxs-lookup"><span data-stu-id="699f6-141">userId</span></span>|<span data-ttu-id="699f6-142">String</span><span class="sxs-lookup"><span data-stu-id="699f6-142">String</span></span>|<span data-ttu-id="699f6-143">用户 id。</span><span class="sxs-lookup"><span data-stu-id="699f6-143">The user ID.</span></span> <span data-ttu-id="699f6-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="699f6-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="699f6-145">userName</span><span class="sxs-lookup"><span data-stu-id="699f6-145">userName</span></span>|<span data-ttu-id="699f6-146">String</span><span class="sxs-lookup"><span data-stu-id="699f6-146">String</span></span>|<span data-ttu-id="699f6-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="699f6-147">The user name.</span></span> <span data-ttu-id="699f6-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="699f6-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="699f6-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="699f6-149">userPrincipalName</span></span>|<span data-ttu-id="699f6-150">字符串</span><span class="sxs-lookup"><span data-stu-id="699f6-150">String</span></span>|<span data-ttu-id="699f6-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="699f6-151">The user principal name.</span></span> <span data-ttu-id="699f6-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="699f6-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="699f6-153">响应</span><span class="sxs-lookup"><span data-stu-id="699f6-153">Response</span></span>
<span data-ttu-id="699f6-154">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="699f6-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="699f6-155">示例</span><span class="sxs-lookup"><span data-stu-id="699f6-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="699f6-156">请求</span><span class="sxs-lookup"><span data-stu-id="699f6-156">Request</span></span>
<span data-ttu-id="699f6-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="699f6-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="699f6-158">响应</span><span class="sxs-lookup"><span data-stu-id="699f6-158">Response</span></span>
<span data-ttu-id="699f6-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="699f6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





