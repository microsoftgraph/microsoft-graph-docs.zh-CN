---
title: 更新 iosVppAppAssignedLicense
description: 更新 iosVppAppAssignedLicense 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 86b618275d1312953d14367d23bbde99aee0cff4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969070"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="a530c-103">更新 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="a530c-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="a530c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a530c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a530c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a530c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a530c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a530c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a530c-107">更新[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a530c-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a530c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a530c-108">Prerequisites</span></span>
<span data-ttu-id="a530c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a530c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a530c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a530c-111">Permission type</span></span>|<span data-ttu-id="a530c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a530c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a530c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a530c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a530c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a530c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a530c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a530c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a530c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a530c-116">Not supported.</span></span>|
|<span data-ttu-id="a530c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a530c-117">Application</span></span>|<span data-ttu-id="a530c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a530c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a530c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a530c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="a530c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a530c-120">Request headers</span></span>
|<span data-ttu-id="a530c-121">标头</span><span class="sxs-lookup"><span data-stu-id="a530c-121">Header</span></span>|<span data-ttu-id="a530c-122">值</span><span class="sxs-lookup"><span data-stu-id="a530c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a530c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a530c-123">Authorization</span></span>|<span data-ttu-id="a530c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a530c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a530c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a530c-125">Accept</span></span>|<span data-ttu-id="a530c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a530c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a530c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a530c-127">Request body</span></span>
<span data-ttu-id="a530c-128">在请求正文中，提供[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a530c-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="a530c-129">下表显示时创建[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a530c-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="a530c-130">属性</span><span class="sxs-lookup"><span data-stu-id="a530c-130">Property</span></span>|<span data-ttu-id="a530c-131">类型</span><span class="sxs-lookup"><span data-stu-id="a530c-131">Type</span></span>|<span data-ttu-id="a530c-132">说明</span><span class="sxs-lookup"><span data-stu-id="a530c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a530c-133">id</span><span class="sxs-lookup"><span data-stu-id="a530c-133">id</span></span>|<span data-ttu-id="a530c-134">String</span><span class="sxs-lookup"><span data-stu-id="a530c-134">String</span></span>|<span data-ttu-id="a530c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a530c-135">Key of the entity.</span></span>|
|<span data-ttu-id="a530c-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a530c-136">userEmailAddress</span></span>|<span data-ttu-id="a530c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a530c-137">String</span></span>|<span data-ttu-id="a530c-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a530c-138">The user email address.</span></span>|
|<span data-ttu-id="a530c-139">userId</span><span class="sxs-lookup"><span data-stu-id="a530c-139">userId</span></span>|<span data-ttu-id="a530c-140">String</span><span class="sxs-lookup"><span data-stu-id="a530c-140">String</span></span>|<span data-ttu-id="a530c-141">用户 id。</span><span class="sxs-lookup"><span data-stu-id="a530c-141">The user ID.</span></span>|
|<span data-ttu-id="a530c-142">userName</span><span class="sxs-lookup"><span data-stu-id="a530c-142">userName</span></span>|<span data-ttu-id="a530c-143">String</span><span class="sxs-lookup"><span data-stu-id="a530c-143">String</span></span>|<span data-ttu-id="a530c-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="a530c-144">The user name.</span></span>|
|<span data-ttu-id="a530c-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a530c-145">userPrincipalName</span></span>|<span data-ttu-id="a530c-146">字符串</span><span class="sxs-lookup"><span data-stu-id="a530c-146">String</span></span>|<span data-ttu-id="a530c-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a530c-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="a530c-148">响应</span><span class="sxs-lookup"><span data-stu-id="a530c-148">Response</span></span>
<span data-ttu-id="a530c-149">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a530c-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a530c-150">示例</span><span class="sxs-lookup"><span data-stu-id="a530c-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="a530c-151">请求</span><span class="sxs-lookup"><span data-stu-id="a530c-151">Request</span></span>
<span data-ttu-id="a530c-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a530c-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 171

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a530c-153">响应</span><span class="sxs-lookup"><span data-stu-id="a530c-153">Response</span></span>
<span data-ttu-id="a530c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a530c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





