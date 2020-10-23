---
title: 更新 mobileAppCategory
description: 更新 mobileAppCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d485331b7be97cecae4369a3625c1510e73a389
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685385"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="81027-103">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="81027-103">Update mobileAppCategory</span></span>

<span data-ttu-id="81027-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81027-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81027-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81027-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81027-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81027-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81027-107">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="81027-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81027-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="81027-108">Prerequisites</span></span>
<span data-ttu-id="81027-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81027-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="81027-111">Permission type</span></span>|<span data-ttu-id="81027-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="81027-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81027-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81027-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81027-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81027-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81027-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81027-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81027-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="81027-116">Not supported.</span></span>|
|<span data-ttu-id="81027-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="81027-117">Application</span></span>|<span data-ttu-id="81027-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81027-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81027-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81027-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="81027-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="81027-120">Request headers</span></span>
|<span data-ttu-id="81027-121">标头</span><span class="sxs-lookup"><span data-stu-id="81027-121">Header</span></span>|<span data-ttu-id="81027-122">值</span><span class="sxs-lookup"><span data-stu-id="81027-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81027-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81027-123">Authorization</span></span>|<span data-ttu-id="81027-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="81027-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81027-125">接受</span><span class="sxs-lookup"><span data-stu-id="81027-125">Accept</span></span>|<span data-ttu-id="81027-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81027-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81027-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="81027-127">Request body</span></span>
<span data-ttu-id="81027-128">在请求正文中，提供 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81027-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="81027-129">下表显示创建 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="81027-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="81027-130">属性</span><span class="sxs-lookup"><span data-stu-id="81027-130">Property</span></span>|<span data-ttu-id="81027-131">类型</span><span class="sxs-lookup"><span data-stu-id="81027-131">Type</span></span>|<span data-ttu-id="81027-132">说明</span><span class="sxs-lookup"><span data-stu-id="81027-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81027-133">id</span><span class="sxs-lookup"><span data-stu-id="81027-133">id</span></span>|<span data-ttu-id="81027-134">String</span><span class="sxs-lookup"><span data-stu-id="81027-134">String</span></span>|<span data-ttu-id="81027-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81027-135">The key of the entity.</span></span>|
|<span data-ttu-id="81027-136">displayName</span><span class="sxs-lookup"><span data-stu-id="81027-136">displayName</span></span>|<span data-ttu-id="81027-137">String</span><span class="sxs-lookup"><span data-stu-id="81027-137">String</span></span>|<span data-ttu-id="81027-138">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="81027-138">The name of the app category.</span></span>|
|<span data-ttu-id="81027-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81027-139">lastModifiedDateTime</span></span>|<span data-ttu-id="81027-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81027-140">DateTimeOffset</span></span>|<span data-ttu-id="81027-141">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81027-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="81027-142">响应</span><span class="sxs-lookup"><span data-stu-id="81027-142">Response</span></span>
<span data-ttu-id="81027-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81027-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81027-144">示例</span><span class="sxs-lookup"><span data-stu-id="81027-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="81027-145">请求</span><span class="sxs-lookup"><span data-stu-id="81027-145">Request</span></span>
<span data-ttu-id="81027-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81027-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="81027-147">响应</span><span class="sxs-lookup"><span data-stu-id="81027-147">Response</span></span>
<span data-ttu-id="81027-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="81027-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





