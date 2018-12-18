---
title: 列出 targetedManagedAppConfigurations
description: 列出 targetedManagedAppConfiguration 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: fc9b6bd3c2851a46ebbdb5bfe4929f8609ed5a2f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324043"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="b0958-103">列出 targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="b0958-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="b0958-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b0958-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0958-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b0958-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0958-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0958-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0958-107">列出 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0958-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0958-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0958-108">Prerequisites</span></span>
<span data-ttu-id="b0958-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b0958-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0958-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0958-111">Permission type</span></span>|<span data-ttu-id="b0958-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0958-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0958-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0958-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0958-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0958-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0958-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0958-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0958-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0958-116">Not supported.</span></span>|
|<span data-ttu-id="b0958-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0958-117">Application</span></span>|<span data-ttu-id="b0958-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0958-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0958-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0958-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0958-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0958-120">Request headers</span></span>
|<span data-ttu-id="b0958-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0958-121">Header</span></span>|<span data-ttu-id="b0958-122">值</span><span class="sxs-lookup"><span data-stu-id="b0958-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0958-123">授权</span><span class="sxs-lookup"><span data-stu-id="b0958-123">Authorization</span></span>|<span data-ttu-id="b0958-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0958-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0958-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0958-125">Accept</span></span>|<span data-ttu-id="b0958-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0958-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0958-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0958-127">Request body</span></span>
<span data-ttu-id="b0958-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0958-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0958-129">响应</span><span class="sxs-lookup"><span data-stu-id="b0958-129">Response</span></span>
<span data-ttu-id="b0958-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b0958-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0958-131">示例</span><span class="sxs-lookup"><span data-stu-id="b0958-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0958-132">请求</span><span class="sxs-lookup"><span data-stu-id="b0958-132">Request</span></span>
<span data-ttu-id="b0958-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0958-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="b0958-134">响应</span><span class="sxs-lookup"><span data-stu-id="b0958-134">Response</span></span>
<span data-ttu-id="b0958-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0958-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```





