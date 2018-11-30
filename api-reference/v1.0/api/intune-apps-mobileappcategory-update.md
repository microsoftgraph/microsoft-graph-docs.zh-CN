---
title: 更新 mobileAppCategory
description: 更新 mobileAppCategory 对象的属性。
ms.openlocfilehash: dee39cf60590f18547d54ea07f96fd7c194a631c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008758"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="abb26-103">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="abb26-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="abb26-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="abb26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abb26-105">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="abb26-105">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abb26-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="abb26-106">Prerequisites</span></span>
<span data-ttu-id="abb26-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="abb26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb26-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb26-109">Permission type</span></span>|<span data-ttu-id="abb26-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="abb26-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb26-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="abb26-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb26-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abb26-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb26-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb26-114">Not supported.</span></span>|
|<span data-ttu-id="abb26-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb26-115">Application</span></span>|<span data-ttu-id="abb26-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb26-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb26-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb26-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="abb26-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb26-118">Request headers</span></span>
|<span data-ttu-id="abb26-119">标头</span><span class="sxs-lookup"><span data-stu-id="abb26-119">Header</span></span>|<span data-ttu-id="abb26-120">值</span><span class="sxs-lookup"><span data-stu-id="abb26-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abb26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb26-121">Authorization</span></span>|<span data-ttu-id="abb26-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="abb26-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abb26-123">Accept</span><span class="sxs-lookup"><span data-stu-id="abb26-123">Accept</span></span>|<span data-ttu-id="abb26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="abb26-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb26-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb26-125">Request body</span></span>
<span data-ttu-id="abb26-126">在请求正文中，提供 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abb26-126">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="abb26-127">下表显示创建 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="abb26-127">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="abb26-128">属性</span><span class="sxs-lookup"><span data-stu-id="abb26-128">Property</span></span>|<span data-ttu-id="abb26-129">类型</span><span class="sxs-lookup"><span data-stu-id="abb26-129">Type</span></span>|<span data-ttu-id="abb26-130">说明</span><span class="sxs-lookup"><span data-stu-id="abb26-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abb26-131">id</span><span class="sxs-lookup"><span data-stu-id="abb26-131">id</span></span>|<span data-ttu-id="abb26-132">String</span><span class="sxs-lookup"><span data-stu-id="abb26-132">String</span></span>|<span data-ttu-id="abb26-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="abb26-133">The key of the entity.</span></span>|
|<span data-ttu-id="abb26-134">displayName</span><span class="sxs-lookup"><span data-stu-id="abb26-134">displayName</span></span>|<span data-ttu-id="abb26-135">String</span><span class="sxs-lookup"><span data-stu-id="abb26-135">String</span></span>|<span data-ttu-id="abb26-136">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="abb26-136">The name of the app category.</span></span>|
|<span data-ttu-id="abb26-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abb26-137">lastModifiedDateTime</span></span>|<span data-ttu-id="abb26-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abb26-138">DateTimeOffset</span></span>|<span data-ttu-id="abb26-139">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="abb26-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="abb26-140">响应</span><span class="sxs-lookup"><span data-stu-id="abb26-140">Response</span></span>
<span data-ttu-id="abb26-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abb26-141">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb26-142">示例</span><span class="sxs-lookup"><span data-stu-id="abb26-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="abb26-143">请求</span><span class="sxs-lookup"><span data-stu-id="abb26-143">Request</span></span>
<span data-ttu-id="abb26-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abb26-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="abb26-145">响应</span><span class="sxs-lookup"><span data-stu-id="abb26-145">Response</span></span>
<span data-ttu-id="abb26-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="abb26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



