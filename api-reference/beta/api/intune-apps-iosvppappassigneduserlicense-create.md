---
title: 创建 iosVppAppAssignedUserLicense
description: 创建新的 iosVppAppAssignedUserLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2e6178570da6e89ef50c933d027daa2a9d7e1adf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864650"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="adba8-103">创建 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="adba8-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="adba8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="adba8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adba8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="adba8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adba8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="adba8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adba8-107">创建新的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adba8-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adba8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="adba8-108">Prerequisites</span></span>
<span data-ttu-id="adba8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="adba8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adba8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="adba8-111">Permission type</span></span>|<span data-ttu-id="adba8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="adba8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adba8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adba8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adba8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adba8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="adba8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adba8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adba8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="adba8-116">Not supported.</span></span>|
|<span data-ttu-id="adba8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="adba8-117">Application</span></span>|<span data-ttu-id="adba8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="adba8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adba8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adba8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="adba8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="adba8-120">Request headers</span></span>
|<span data-ttu-id="adba8-121">标头</span><span class="sxs-lookup"><span data-stu-id="adba8-121">Header</span></span>|<span data-ttu-id="adba8-122">值</span><span class="sxs-lookup"><span data-stu-id="adba8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adba8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adba8-123">Authorization</span></span>|<span data-ttu-id="adba8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="adba8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adba8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="adba8-125">Accept</span></span>|<span data-ttu-id="adba8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adba8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adba8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="adba8-127">Request body</span></span>
<span data-ttu-id="adba8-128">在请求正文中，提供 iosVppAppAssignedUserLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adba8-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="adba8-129">下表显示时创建 iosVppAppAssignedUserLicense 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="adba8-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="adba8-130">属性</span><span class="sxs-lookup"><span data-stu-id="adba8-130">Property</span></span>|<span data-ttu-id="adba8-131">类型</span><span class="sxs-lookup"><span data-stu-id="adba8-131">Type</span></span>|<span data-ttu-id="adba8-132">说明</span><span class="sxs-lookup"><span data-stu-id="adba8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adba8-133">id</span><span class="sxs-lookup"><span data-stu-id="adba8-133">id</span></span>|<span data-ttu-id="adba8-134">String</span><span class="sxs-lookup"><span data-stu-id="adba8-134">String</span></span>|<span data-ttu-id="adba8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="adba8-135">Key of the entity.</span></span> <span data-ttu-id="adba8-136">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="adba8-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="adba8-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="adba8-137">userEmailAddress</span></span>|<span data-ttu-id="adba8-138">字符串</span><span class="sxs-lookup"><span data-stu-id="adba8-138">String</span></span>|<span data-ttu-id="adba8-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="adba8-139">The user email address.</span></span> <span data-ttu-id="adba8-140">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="adba8-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="adba8-141">userId</span><span class="sxs-lookup"><span data-stu-id="adba8-141">userId</span></span>|<span data-ttu-id="adba8-142">String</span><span class="sxs-lookup"><span data-stu-id="adba8-142">String</span></span>|<span data-ttu-id="adba8-143">用户 id。</span><span class="sxs-lookup"><span data-stu-id="adba8-143">The user ID.</span></span> <span data-ttu-id="adba8-144">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="adba8-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="adba8-145">userName</span><span class="sxs-lookup"><span data-stu-id="adba8-145">userName</span></span>|<span data-ttu-id="adba8-146">String</span><span class="sxs-lookup"><span data-stu-id="adba8-146">String</span></span>|<span data-ttu-id="adba8-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="adba8-147">The user name.</span></span> <span data-ttu-id="adba8-148">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="adba8-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="adba8-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="adba8-149">userPrincipalName</span></span>|<span data-ttu-id="adba8-150">字符串</span><span class="sxs-lookup"><span data-stu-id="adba8-150">String</span></span>|<span data-ttu-id="adba8-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="adba8-151">The user principal name.</span></span> <span data-ttu-id="adba8-152">继承自[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="adba8-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="adba8-153">响应</span><span class="sxs-lookup"><span data-stu-id="adba8-153">Response</span></span>
<span data-ttu-id="adba8-154">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adba8-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adba8-155">示例</span><span class="sxs-lookup"><span data-stu-id="adba8-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="adba8-156">请求</span><span class="sxs-lookup"><span data-stu-id="adba8-156">Request</span></span>
<span data-ttu-id="adba8-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="adba8-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="adba8-158">响应</span><span class="sxs-lookup"><span data-stu-id="adba8-158">Response</span></span>
<span data-ttu-id="adba8-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adba8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





