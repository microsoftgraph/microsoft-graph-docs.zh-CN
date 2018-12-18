---
title: 列出 iosMobileAppConfigurations
description: 列出 iosMobileAppConfiguration 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: ecf23edce97954f0c6305e9a49503b857479728a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302238"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="bbee1-103">列出 iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="bbee1-103">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="bbee1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bbee1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbee1-105">列出 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bbee1-105">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbee1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbee1-106">Prerequisites</span></span>
<span data-ttu-id="bbee1-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bbee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbee1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbee1-109">Permission type</span></span>|<span data-ttu-id="bbee1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bbee1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbee1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbee1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bbee1-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbee1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bbee1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbee1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbee1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbee1-114">Not supported.</span></span>|
|<span data-ttu-id="bbee1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbee1-115">Application</span></span>|<span data-ttu-id="bbee1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbee1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbee1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbee1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bbee1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbee1-118">Request headers</span></span>
|<span data-ttu-id="bbee1-119">标头</span><span class="sxs-lookup"><span data-stu-id="bbee1-119">Header</span></span>|<span data-ttu-id="bbee1-120">值</span><span class="sxs-lookup"><span data-stu-id="bbee1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbee1-121">授权</span><span class="sxs-lookup"><span data-stu-id="bbee1-121">Authorization</span></span>|<span data-ttu-id="bbee1-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbee1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbee1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bbee1-123">Accept</span></span>|<span data-ttu-id="bbee1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bbee1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbee1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbee1-125">Request body</span></span>
<span data-ttu-id="bbee1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbee1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbee1-127">响应</span><span class="sxs-lookup"><span data-stu-id="bbee1-127">Response</span></span>
<span data-ttu-id="bbee1-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bbee1-128">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbee1-129">示例</span><span class="sxs-lookup"><span data-stu-id="bbee1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbee1-130">请求</span><span class="sxs-lookup"><span data-stu-id="bbee1-130">Request</span></span>
<span data-ttu-id="bbee1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbee1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="bbee1-132">响应</span><span class="sxs-lookup"><span data-stu-id="bbee1-132">Response</span></span>
<span data-ttu-id="bbee1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbee1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
      "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
      "settings": [
        {
          "@odata.type": "microsoft.graph.appConfigurationSettingItem",
          "appConfigKey": "App Config Key value",
          "appConfigKeyType": "integerType",
          "appConfigKeyValue": "App Config Key Value value"
        }
      ]
    }
  ]
}
```



