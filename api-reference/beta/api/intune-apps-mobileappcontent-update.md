---
title: 更新 mobileAppContent
description: 更新 mobileAppContent 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 262a7fc48e30e816b07aae963a0951ed4605925d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413372"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="e69c3-103">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e69c3-103">Update mobileAppContent</span></span>

> <span data-ttu-id="e69c3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e69c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e69c3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e69c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e69c3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e69c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e69c3-107">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e69c3-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e69c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e69c3-108">Prerequisites</span></span>
<span data-ttu-id="e69c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e69c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e69c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e69c3-111">Permission type</span></span>|<span data-ttu-id="e69c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e69c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e69c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e69c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e69c3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e69c3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e69c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e69c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e69c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e69c3-116">Not supported.</span></span>|
|<span data-ttu-id="e69c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e69c3-117">Application</span></span>|<span data-ttu-id="e69c3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e69c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e69c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e69c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="e69c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e69c3-120">Request headers</span></span>
|<span data-ttu-id="e69c3-121">标头</span><span class="sxs-lookup"><span data-stu-id="e69c3-121">Header</span></span>|<span data-ttu-id="e69c3-122">值</span><span class="sxs-lookup"><span data-stu-id="e69c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e69c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e69c3-123">Authorization</span></span>|<span data-ttu-id="e69c3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e69c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e69c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e69c3-125">Accept</span></span>|<span data-ttu-id="e69c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e69c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e69c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e69c3-127">Request body</span></span>
<span data-ttu-id="e69c3-128">在请求正文中，提供 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e69c3-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="e69c3-129">下表显示创建 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e69c3-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="e69c3-130">属性</span><span class="sxs-lookup"><span data-stu-id="e69c3-130">Property</span></span>|<span data-ttu-id="e69c3-131">类型</span><span class="sxs-lookup"><span data-stu-id="e69c3-131">Type</span></span>|<span data-ttu-id="e69c3-132">说明</span><span class="sxs-lookup"><span data-stu-id="e69c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e69c3-133">id</span><span class="sxs-lookup"><span data-stu-id="e69c3-133">id</span></span>|<span data-ttu-id="e69c3-134">String</span><span class="sxs-lookup"><span data-stu-id="e69c3-134">String</span></span>|<span data-ttu-id="e69c3-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="e69c3-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="e69c3-136">响应</span><span class="sxs-lookup"><span data-stu-id="e69c3-136">Response</span></span>
<span data-ttu-id="e69c3-137">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e69c3-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e69c3-138">示例</span><span class="sxs-lookup"><span data-stu-id="e69c3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e69c3-139">请求</span><span class="sxs-lookup"><span data-stu-id="e69c3-139">Request</span></span>
<span data-ttu-id="e69c3-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e69c3-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="e69c3-141">响应</span><span class="sxs-lookup"><span data-stu-id="e69c3-141">Response</span></span>
<span data-ttu-id="e69c3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e69c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




