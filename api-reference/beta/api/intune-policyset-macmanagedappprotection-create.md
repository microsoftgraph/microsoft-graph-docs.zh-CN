---
title: 创建 macManagedAppProtection
description: 创建新的 macManagedAppProtection 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb021c1d68acb30554d879b8f77e5bbf77c46ff8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191976"
---
# <a name="create-macmanagedappprotection"></a><span data-ttu-id="c6f1d-103">创建 macManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c6f1d-103">Create macManagedAppProtection</span></span>

> <span data-ttu-id="c6f1d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6f1d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6f1d-106">创建新的[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-106">Create a new [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6f1d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6f1d-107">Prerequisites</span></span>
<span data-ttu-id="c6f1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f1d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6f1d-110">Permission type</span></span>|<span data-ttu-id="c6f1d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6f1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6f1d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6f1d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f1d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6f1d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6f1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-115">Not supported.</span></span>|
|<span data-ttu-id="c6f1d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6f1d-116">Application</span></span>|<span data-ttu-id="c6f1d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f1d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6f1d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6f1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/macManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="c6f1d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6f1d-119">Request headers</span></span>
|<span data-ttu-id="c6f1d-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6f1d-120">Header</span></span>|<span data-ttu-id="c6f1d-121">值</span><span class="sxs-lookup"><span data-stu-id="c6f1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6f1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6f1d-122">Authorization</span></span>|<span data-ttu-id="c6f1d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6f1d-124">接受</span><span class="sxs-lookup"><span data-stu-id="c6f1d-124">Accept</span></span>|<span data-ttu-id="c6f1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6f1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6f1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6f1d-126">Request body</span></span>
<span data-ttu-id="c6f1d-127">在请求正文中，提供 macManagedAppProtection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-127">In the request body, supply a JSON representation for the macManagedAppProtection object.</span></span>

<span data-ttu-id="c6f1d-128">下表显示创建 macManagedAppProtection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-128">The following table shows the properties that are required when you create the macManagedAppProtection.</span></span>

|<span data-ttu-id="c6f1d-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6f1d-129">Property</span></span>|<span data-ttu-id="c6f1d-130">类型</span><span class="sxs-lookup"><span data-stu-id="c6f1d-130">Type</span></span>|<span data-ttu-id="c6f1d-131">说明</span><span class="sxs-lookup"><span data-stu-id="c6f1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6f1d-132">id</span><span class="sxs-lookup"><span data-stu-id="c6f1d-132">id</span></span>|<span data-ttu-id="c6f1d-133">String</span><span class="sxs-lookup"><span data-stu-id="c6f1d-133">String</span></span>|<span data-ttu-id="c6f1d-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c6f1d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c6f1d-135">响应</span><span class="sxs-lookup"><span data-stu-id="c6f1d-135">Response</span></span>
<span data-ttu-id="c6f1d-136">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-136">If successful, this method returns a `201 Created` response code and a [macManagedAppProtection](../resources/intune-policyset-macmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6f1d-137">示例</span><span class="sxs-lookup"><span data-stu-id="c6f1d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6f1d-138">请求</span><span class="sxs-lookup"><span data-stu-id="c6f1d-138">Request</span></span>
<span data-ttu-id="c6f1d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/macManagedAppProtections
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.macManagedAppProtection"
}
```

### <a name="response"></a><span data-ttu-id="c6f1d-140">响应</span><span class="sxs-lookup"><span data-stu-id="c6f1d-140">Response</span></span>
<span data-ttu-id="c6f1d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6f1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.macManagedAppProtection",
  "id": "bb139531-9531-bb13-3195-13bb319513bb"
}
```




