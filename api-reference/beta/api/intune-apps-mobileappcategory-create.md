---
title: 创建 mobileAppCategory
description: 创建新的 mobileAppCategory 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d71c7f9452f65d40fea6b0e5141916560a0c9f01
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974165"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="ae164-103">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="ae164-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="ae164-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ae164-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae164-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae164-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae164-106">创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae164-106">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae164-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ae164-107">Prerequisites</span></span>
<span data-ttu-id="ae164-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae164-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae164-110">Permission type</span></span>|<span data-ttu-id="ae164-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ae164-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae164-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae164-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae164-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae164-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae164-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae164-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae164-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae164-115">Not supported.</span></span>|
|<span data-ttu-id="ae164-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae164-116">Application</span></span>|<span data-ttu-id="ae164-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae164-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae164-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae164-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="ae164-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae164-119">Request headers</span></span>
|<span data-ttu-id="ae164-120">标头</span><span class="sxs-lookup"><span data-stu-id="ae164-120">Header</span></span>|<span data-ttu-id="ae164-121">值</span><span class="sxs-lookup"><span data-stu-id="ae164-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae164-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae164-122">Authorization</span></span>|<span data-ttu-id="ae164-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ae164-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae164-124">接受</span><span class="sxs-lookup"><span data-stu-id="ae164-124">Accept</span></span>|<span data-ttu-id="ae164-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae164-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae164-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae164-126">Request body</span></span>
<span data-ttu-id="ae164-127">在请求正文中，提供 mobileAppCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae164-127">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="ae164-128">下表显示创建 mobileAppCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ae164-128">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="ae164-129">属性</span><span class="sxs-lookup"><span data-stu-id="ae164-129">Property</span></span>|<span data-ttu-id="ae164-130">类型</span><span class="sxs-lookup"><span data-stu-id="ae164-130">Type</span></span>|<span data-ttu-id="ae164-131">说明</span><span class="sxs-lookup"><span data-stu-id="ae164-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae164-132">id</span><span class="sxs-lookup"><span data-stu-id="ae164-132">id</span></span>|<span data-ttu-id="ae164-133">String</span><span class="sxs-lookup"><span data-stu-id="ae164-133">String</span></span>|<span data-ttu-id="ae164-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ae164-134">The key of the entity.</span></span>|
|<span data-ttu-id="ae164-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ae164-135">displayName</span></span>|<span data-ttu-id="ae164-136">String</span><span class="sxs-lookup"><span data-stu-id="ae164-136">String</span></span>|<span data-ttu-id="ae164-137">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="ae164-137">The name of the app category.</span></span>|
|<span data-ttu-id="ae164-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae164-138">lastModifiedDateTime</span></span>|<span data-ttu-id="ae164-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae164-139">DateTimeOffset</span></span>|<span data-ttu-id="ae164-140">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ae164-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ae164-141">响应</span><span class="sxs-lookup"><span data-stu-id="ae164-141">Response</span></span>
<span data-ttu-id="ae164-142">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae164-142">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae164-143">示例</span><span class="sxs-lookup"><span data-stu-id="ae164-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae164-144">请求</span><span class="sxs-lookup"><span data-stu-id="ae164-144">Request</span></span>
<span data-ttu-id="ae164-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae164-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ae164-146">响应</span><span class="sxs-lookup"><span data-stu-id="ae164-146">Response</span></span>
<span data-ttu-id="ae164-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae164-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





