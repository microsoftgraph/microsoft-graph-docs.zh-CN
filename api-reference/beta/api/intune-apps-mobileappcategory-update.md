---
title: 更新 mobileAppCategory
description: 更新 mobileAppCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d19dcdb6c4223df10b657d2e599d7803878a82c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143295"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="615e4-103">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="615e4-103">Update mobileAppCategory</span></span>

<span data-ttu-id="615e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="615e4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="615e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="615e4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="615e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="615e4-107">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="615e4-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="615e4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="615e4-108">Prerequisites</span></span>
<span data-ttu-id="615e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="615e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="615e4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="615e4-111">Permission type</span></span>|<span data-ttu-id="615e4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="615e4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="615e4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="615e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="615e4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615e4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="615e4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="615e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="615e4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="615e4-116">Not supported.</span></span>|
|<span data-ttu-id="615e4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="615e4-117">Application</span></span>|<span data-ttu-id="615e4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615e4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="615e4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="615e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="615e4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="615e4-120">Request headers</span></span>
|<span data-ttu-id="615e4-121">标头</span><span class="sxs-lookup"><span data-stu-id="615e4-121">Header</span></span>|<span data-ttu-id="615e4-122">值</span><span class="sxs-lookup"><span data-stu-id="615e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="615e4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="615e4-123">Authorization</span></span>|<span data-ttu-id="615e4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="615e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="615e4-125">接受</span><span class="sxs-lookup"><span data-stu-id="615e4-125">Accept</span></span>|<span data-ttu-id="615e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="615e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="615e4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="615e4-127">Request body</span></span>
<span data-ttu-id="615e4-128">在请求正文中，提供 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="615e4-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="615e4-129">下表显示创建 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="615e4-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="615e4-130">属性</span><span class="sxs-lookup"><span data-stu-id="615e4-130">Property</span></span>|<span data-ttu-id="615e4-131">类型</span><span class="sxs-lookup"><span data-stu-id="615e4-131">Type</span></span>|<span data-ttu-id="615e4-132">说明</span><span class="sxs-lookup"><span data-stu-id="615e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="615e4-133">id</span><span class="sxs-lookup"><span data-stu-id="615e4-133">id</span></span>|<span data-ttu-id="615e4-134">String</span><span class="sxs-lookup"><span data-stu-id="615e4-134">String</span></span>|<span data-ttu-id="615e4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="615e4-135">The key of the entity.</span></span>|
|<span data-ttu-id="615e4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="615e4-136">displayName</span></span>|<span data-ttu-id="615e4-137">String</span><span class="sxs-lookup"><span data-stu-id="615e4-137">String</span></span>|<span data-ttu-id="615e4-138">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="615e4-138">The name of the app category.</span></span>|
|<span data-ttu-id="615e4-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="615e4-139">lastModifiedDateTime</span></span>|<span data-ttu-id="615e4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615e4-140">DateTimeOffset</span></span>|<span data-ttu-id="615e4-141">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="615e4-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="615e4-142">响应</span><span class="sxs-lookup"><span data-stu-id="615e4-142">Response</span></span>
<span data-ttu-id="615e4-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="615e4-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="615e4-144">示例</span><span class="sxs-lookup"><span data-stu-id="615e4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="615e4-145">请求</span><span class="sxs-lookup"><span data-stu-id="615e4-145">Request</span></span>
<span data-ttu-id="615e4-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="615e4-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="615e4-147">响应</span><span class="sxs-lookup"><span data-stu-id="615e4-147">Response</span></span>
<span data-ttu-id="615e4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="615e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




