---
title: 创建 mobileAppCategory
description: 创建新的 mobileAppCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1f9cbb590124c5425feca3bf9941fc396de78ce
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692294"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="9fced-103">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="9fced-103">Create mobileAppCategory</span></span>

<span data-ttu-id="9fced-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fced-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fced-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fced-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fced-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fced-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fced-107">创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fced-107">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fced-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9fced-108">Prerequisites</span></span>
<span data-ttu-id="9fced-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fced-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fced-111">Permission type</span></span>|<span data-ttu-id="9fced-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9fced-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fced-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fced-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fced-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fced-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fced-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fced-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fced-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fced-116">Not supported.</span></span>|
|<span data-ttu-id="9fced-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fced-117">Application</span></span>|<span data-ttu-id="9fced-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fced-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fced-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fced-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="9fced-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fced-120">Request headers</span></span>
|<span data-ttu-id="9fced-121">标头</span><span class="sxs-lookup"><span data-stu-id="9fced-121">Header</span></span>|<span data-ttu-id="9fced-122">值</span><span class="sxs-lookup"><span data-stu-id="9fced-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fced-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fced-123">Authorization</span></span>|<span data-ttu-id="9fced-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9fced-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fced-125">接受</span><span class="sxs-lookup"><span data-stu-id="9fced-125">Accept</span></span>|<span data-ttu-id="9fced-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fced-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fced-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fced-127">Request body</span></span>
<span data-ttu-id="9fced-128">在请求正文中，提供 mobileAppCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fced-128">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="9fced-129">下表显示创建 mobileAppCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9fced-129">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="9fced-130">属性</span><span class="sxs-lookup"><span data-stu-id="9fced-130">Property</span></span>|<span data-ttu-id="9fced-131">类型</span><span class="sxs-lookup"><span data-stu-id="9fced-131">Type</span></span>|<span data-ttu-id="9fced-132">说明</span><span class="sxs-lookup"><span data-stu-id="9fced-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fced-133">id</span><span class="sxs-lookup"><span data-stu-id="9fced-133">id</span></span>|<span data-ttu-id="9fced-134">String</span><span class="sxs-lookup"><span data-stu-id="9fced-134">String</span></span>|<span data-ttu-id="9fced-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9fced-135">The key of the entity.</span></span>|
|<span data-ttu-id="9fced-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9fced-136">displayName</span></span>|<span data-ttu-id="9fced-137">String</span><span class="sxs-lookup"><span data-stu-id="9fced-137">String</span></span>|<span data-ttu-id="9fced-138">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="9fced-138">The name of the app category.</span></span>|
|<span data-ttu-id="9fced-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fced-139">lastModifiedDateTime</span></span>|<span data-ttu-id="9fced-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fced-140">DateTimeOffset</span></span>|<span data-ttu-id="9fced-141">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9fced-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9fced-142">响应</span><span class="sxs-lookup"><span data-stu-id="9fced-142">Response</span></span>
<span data-ttu-id="9fced-143">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fced-143">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fced-144">示例</span><span class="sxs-lookup"><span data-stu-id="9fced-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fced-145">请求</span><span class="sxs-lookup"><span data-stu-id="9fced-145">Request</span></span>
<span data-ttu-id="9fced-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fced-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="9fced-147">响应</span><span class="sxs-lookup"><span data-stu-id="9fced-147">Response</span></span>
<span data-ttu-id="9fced-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fced-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





