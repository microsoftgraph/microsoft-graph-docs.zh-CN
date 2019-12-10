---
title: 获取 androidManagedStoreAccountEnterpriseSettings
description: 读取 androidManagedStoreAccountEnterpriseSettings 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6aa8ca6f7795ba521031d75e583e10bdb835690
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39922921"
---
# <a name="get-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="6a4a3-103">获取 androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="6a4a3-103">Get androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="6a4a3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a4a3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a4a3-106">读取[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-106">Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a4a3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a4a3-107">Prerequisites</span></span>
<span data-ttu-id="6a4a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a4a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a4a3-110">Permission type</span></span>|<span data-ttu-id="6a4a3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a4a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a4a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a4a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a4a3-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a4a3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6a4a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a4a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a4a3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-115">Not supported.</span></span>|
|<span data-ttu-id="6a4a3-116">Application</span><span class="sxs-lookup"><span data-stu-id="6a4a3-116">Application</span></span>|<span data-ttu-id="6a4a3-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a4a3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a4a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a4a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a4a3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6a4a3-119">Optional query parameters</span></span>
<span data-ttu-id="6a4a3-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a4a3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a4a3-121">Request headers</span></span>
|<span data-ttu-id="6a4a3-122">标头</span><span class="sxs-lookup"><span data-stu-id="6a4a3-122">Header</span></span>|<span data-ttu-id="6a4a3-123">值</span><span class="sxs-lookup"><span data-stu-id="6a4a3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a4a3-124">授权</span><span class="sxs-lookup"><span data-stu-id="6a4a3-124">Authorization</span></span>|<span data-ttu-id="6a4a3-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a4a3-126">接受</span><span class="sxs-lookup"><span data-stu-id="6a4a3-126">Accept</span></span>|<span data-ttu-id="6a4a3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6a4a3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a4a3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a4a3-128">Request body</span></span>
<span data-ttu-id="6a4a3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a4a3-130">响应</span><span class="sxs-lookup"><span data-stu-id="6a4a3-130">Response</span></span>
<span data-ttu-id="6a4a3-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a4a3-132">示例</span><span class="sxs-lookup"><span data-stu-id="6a4a3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a4a3-133">请求</span><span class="sxs-lookup"><span data-stu-id="6a4a3-133">Request</span></span>
<span data-ttu-id="6a4a3-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

### <a name="response"></a><span data-ttu-id="6a4a3-135">响应</span><span class="sxs-lookup"><span data-stu-id="6a4a3-135">Response</span></span>
<span data-ttu-id="6a4a3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a4a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1081

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
    "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true,
    "companyCodes": [
      {
        "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
        "enrollmentToken": "Enrollment Token value",
        "qrCodeContent": "Qr Code Content value",
        "qrCodeImage": {
          "@odata.type": "microsoft.graph.mimeContent",
          "type": "Type value",
          "value": "dmFsdWU="
        }
      }
    ],
    "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
  }
}
```





