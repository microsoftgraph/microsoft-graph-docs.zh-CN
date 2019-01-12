---
title: 列出 deviceCategories
description: 列出 deviceCategory 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 410db393c354038f9e0442f10c1a2a9b413533c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949379"
---
# <a name="list-devicecategories"></a><span data-ttu-id="0b44f-103">列出 deviceCategories</span><span class="sxs-lookup"><span data-stu-id="0b44f-103">List deviceCategories</span></span>

> <span data-ttu-id="0b44f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b44f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b44f-105">列出 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b44f-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b44f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b44f-106">Prerequisites</span></span>
<span data-ttu-id="0b44f-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0b44f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b44f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b44f-109">Permission type</span></span>|<span data-ttu-id="0b44f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b44f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b44f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b44f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0b44f-112">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="0b44f-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0b44f-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b44f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0b44f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b44f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b44f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b44f-115">Not supported.</span></span>|
|<span data-ttu-id="0b44f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b44f-116">Application</span></span>|<span data-ttu-id="0b44f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b44f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b44f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b44f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="0b44f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b44f-119">Request headers</span></span>
|<span data-ttu-id="0b44f-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b44f-120">Header</span></span>|<span data-ttu-id="0b44f-121">值</span><span class="sxs-lookup"><span data-stu-id="0b44f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b44f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b44f-122">Authorization</span></span>|<span data-ttu-id="0b44f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b44f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b44f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0b44f-124">Accept</span></span>|<span data-ttu-id="0b44f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b44f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b44f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b44f-126">Request body</span></span>
<span data-ttu-id="0b44f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b44f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b44f-128">响应</span><span class="sxs-lookup"><span data-stu-id="0b44f-128">Response</span></span>
<span data-ttu-id="0b44f-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0b44f-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b44f-130">示例</span><span class="sxs-lookup"><span data-stu-id="0b44f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b44f-131">请求</span><span class="sxs-lookup"><span data-stu-id="0b44f-131">Request</span></span>
<span data-ttu-id="0b44f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b44f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="0b44f-133">响应</span><span class="sxs-lookup"><span data-stu-id="0b44f-133">Response</span></span>
<span data-ttu-id="0b44f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b44f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



