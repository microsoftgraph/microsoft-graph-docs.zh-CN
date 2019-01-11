---
title: 创建 iosVppAppAssignedLicense
description: 创建新的 iosVppAppAssignedLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 225b7168d584faa2e5ff1ec2910fe0e3e53fda8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887099"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="e78b1-103">创建 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="e78b1-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="e78b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e78b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e78b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e78b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e78b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e78b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e78b1-107">创建新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e78b1-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e78b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e78b1-108">Prerequisites</span></span>
<span data-ttu-id="e78b1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e78b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e78b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e78b1-111">Permission type</span></span>|<span data-ttu-id="e78b1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e78b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e78b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e78b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e78b1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78b1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e78b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e78b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e78b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e78b1-116">Not supported.</span></span>|
|<span data-ttu-id="e78b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e78b1-117">Application</span></span>|<span data-ttu-id="e78b1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e78b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e78b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e78b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="e78b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e78b1-120">Request headers</span></span>
|<span data-ttu-id="e78b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="e78b1-121">Header</span></span>|<span data-ttu-id="e78b1-122">值</span><span class="sxs-lookup"><span data-stu-id="e78b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e78b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e78b1-123">Authorization</span></span>|<span data-ttu-id="e78b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e78b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e78b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e78b1-125">Accept</span></span>|<span data-ttu-id="e78b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e78b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e78b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e78b1-127">Request body</span></span>
<span data-ttu-id="e78b1-128">在请求正文中，提供 iosVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e78b1-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="e78b1-129">下表显示时创建 iosVppAppAssignedLicense 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e78b1-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="e78b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="e78b1-130">Property</span></span>|<span data-ttu-id="e78b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="e78b1-131">Type</span></span>|<span data-ttu-id="e78b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="e78b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e78b1-133">id</span><span class="sxs-lookup"><span data-stu-id="e78b1-133">id</span></span>|<span data-ttu-id="e78b1-134">String</span><span class="sxs-lookup"><span data-stu-id="e78b1-134">String</span></span>|<span data-ttu-id="e78b1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e78b1-135">Key of the entity.</span></span>|
|<span data-ttu-id="e78b1-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e78b1-136">userEmailAddress</span></span>|<span data-ttu-id="e78b1-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e78b1-137">String</span></span>|<span data-ttu-id="e78b1-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e78b1-138">The user email address.</span></span>|
|<span data-ttu-id="e78b1-139">userId</span><span class="sxs-lookup"><span data-stu-id="e78b1-139">userId</span></span>|<span data-ttu-id="e78b1-140">String</span><span class="sxs-lookup"><span data-stu-id="e78b1-140">String</span></span>|<span data-ttu-id="e78b1-141">用户 id。</span><span class="sxs-lookup"><span data-stu-id="e78b1-141">The user ID.</span></span>|
|<span data-ttu-id="e78b1-142">userName</span><span class="sxs-lookup"><span data-stu-id="e78b1-142">userName</span></span>|<span data-ttu-id="e78b1-143">String</span><span class="sxs-lookup"><span data-stu-id="e78b1-143">String</span></span>|<span data-ttu-id="e78b1-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="e78b1-144">The user name.</span></span>|
|<span data-ttu-id="e78b1-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e78b1-145">userPrincipalName</span></span>|<span data-ttu-id="e78b1-146">字符串</span><span class="sxs-lookup"><span data-stu-id="e78b1-146">String</span></span>|<span data-ttu-id="e78b1-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e78b1-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="e78b1-148">响应</span><span class="sxs-lookup"><span data-stu-id="e78b1-148">Response</span></span>
<span data-ttu-id="e78b1-149">如果成功，此方法返回`201 Created`响应代码和响应正文中的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e78b1-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e78b1-150">示例</span><span class="sxs-lookup"><span data-stu-id="e78b1-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e78b1-151">请求</span><span class="sxs-lookup"><span data-stu-id="e78b1-151">Request</span></span>
<span data-ttu-id="e78b1-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e78b1-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e78b1-153">响应</span><span class="sxs-lookup"><span data-stu-id="e78b1-153">Response</span></span>
<span data-ttu-id="e78b1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e78b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





