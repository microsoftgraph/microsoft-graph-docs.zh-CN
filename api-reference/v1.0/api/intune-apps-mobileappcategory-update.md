---
title: 更新 mobileAppCategory
description: 更新 mobileAppCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5175886ecb5bd414691050f5fa3cb9cc2ba571a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754091"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="94356-103">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="94356-103">Update mobileAppCategory</span></span>

<span data-ttu-id="94356-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94356-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94356-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94356-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94356-106">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94356-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94356-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="94356-107">Prerequisites</span></span>
<span data-ttu-id="94356-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94356-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94356-110">Permission type</span></span>|<span data-ttu-id="94356-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94356-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94356-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94356-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94356-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94356-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94356-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94356-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94356-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94356-115">Not supported.</span></span>|
|<span data-ttu-id="94356-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94356-116">Application</span></span>|<span data-ttu-id="94356-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94356-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94356-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94356-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="94356-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94356-119">Request headers</span></span>
|<span data-ttu-id="94356-120">标头</span><span class="sxs-lookup"><span data-stu-id="94356-120">Header</span></span>|<span data-ttu-id="94356-121">值</span><span class="sxs-lookup"><span data-stu-id="94356-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94356-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94356-122">Authorization</span></span>|<span data-ttu-id="94356-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="94356-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94356-124">接受</span><span class="sxs-lookup"><span data-stu-id="94356-124">Accept</span></span>|<span data-ttu-id="94356-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94356-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94356-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="94356-126">Request body</span></span>
<span data-ttu-id="94356-127">在请求正文中，提供 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94356-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="94356-128">下表显示创建 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="94356-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="94356-129">属性</span><span class="sxs-lookup"><span data-stu-id="94356-129">Property</span></span>|<span data-ttu-id="94356-130">类型</span><span class="sxs-lookup"><span data-stu-id="94356-130">Type</span></span>|<span data-ttu-id="94356-131">说明</span><span class="sxs-lookup"><span data-stu-id="94356-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94356-132">id</span><span class="sxs-lookup"><span data-stu-id="94356-132">id</span></span>|<span data-ttu-id="94356-133">String</span><span class="sxs-lookup"><span data-stu-id="94356-133">String</span></span>|<span data-ttu-id="94356-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94356-134">The key of the entity.</span></span>|
|<span data-ttu-id="94356-135">displayName</span><span class="sxs-lookup"><span data-stu-id="94356-135">displayName</span></span>|<span data-ttu-id="94356-136">String</span><span class="sxs-lookup"><span data-stu-id="94356-136">String</span></span>|<span data-ttu-id="94356-137">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="94356-137">The name of the app category.</span></span>|
|<span data-ttu-id="94356-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94356-138">lastModifiedDateTime</span></span>|<span data-ttu-id="94356-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94356-139">DateTimeOffset</span></span>|<span data-ttu-id="94356-140">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="94356-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="94356-141">响应</span><span class="sxs-lookup"><span data-stu-id="94356-141">Response</span></span>
<span data-ttu-id="94356-142">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94356-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94356-143">示例</span><span class="sxs-lookup"><span data-stu-id="94356-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="94356-144">请求</span><span class="sxs-lookup"><span data-stu-id="94356-144">Request</span></span>
<span data-ttu-id="94356-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94356-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="94356-146">响应</span><span class="sxs-lookup"><span data-stu-id="94356-146">Response</span></span>
<span data-ttu-id="94356-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94356-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




