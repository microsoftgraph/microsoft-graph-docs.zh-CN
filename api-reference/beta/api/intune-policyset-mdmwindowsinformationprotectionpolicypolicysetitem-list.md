---
title: 列出 mdmWindowsInformationProtectionPolicyPolicySetItems
description: 列出 mdmWindowsInformationProtectionPolicyPolicySetItem 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67fa133f7df2b62d1382967a8772bb7e45919ccd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460729"
---
# <a name="list-mdmwindowsinformationprotectionpolicypolicysetitems"></a><span data-ttu-id="b352c-103">列出 mdmWindowsInformationProtectionPolicyPolicySetItems</span><span class="sxs-lookup"><span data-stu-id="b352c-103">List mdmWindowsInformationProtectionPolicyPolicySetItems</span></span>

<span data-ttu-id="b352c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b352c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b352c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b352c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b352c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b352c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b352c-107">列出[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b352c-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b352c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b352c-108">Prerequisites</span></span>
<span data-ttu-id="b352c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b352c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b352c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b352c-111">Permission type</span></span>|<span data-ttu-id="b352c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b352c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b352c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b352c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b352c-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b352c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b352c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b352c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b352c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b352c-116">Not supported.</span></span>|
|<span data-ttu-id="b352c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b352c-117">Application</span></span>|<span data-ttu-id="b352c-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b352c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b352c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b352c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="b352c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b352c-120">Request headers</span></span>
|<span data-ttu-id="b352c-121">标头</span><span class="sxs-lookup"><span data-stu-id="b352c-121">Header</span></span>|<span data-ttu-id="b352c-122">值</span><span class="sxs-lookup"><span data-stu-id="b352c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b352c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b352c-123">Authorization</span></span>|<span data-ttu-id="b352c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b352c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b352c-125">接受</span><span class="sxs-lookup"><span data-stu-id="b352c-125">Accept</span></span>|<span data-ttu-id="b352c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b352c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b352c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b352c-127">Request body</span></span>
<span data-ttu-id="b352c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b352c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b352c-129">响应</span><span class="sxs-lookup"><span data-stu-id="b352c-129">Response</span></span>
<span data-ttu-id="b352c-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b352c-130">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b352c-131">示例</span><span class="sxs-lookup"><span data-stu-id="b352c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b352c-132">请求</span><span class="sxs-lookup"><span data-stu-id="b352c-132">Request</span></span>
<span data-ttu-id="b352c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b352c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
```

### <a name="response"></a><span data-ttu-id="b352c-134">响应</span><span class="sxs-lookup"><span data-stu-id="b352c-134">Response</span></span>
<span data-ttu-id="b352c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b352c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
      "id": "4ac5be70-be70-4ac5-70be-c54a70bec54a",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "payloadId": "Payload Id value",
      "itemType": "Item Type value",
      "displayName": "Display Name value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ]
    }
  ]
}
```





