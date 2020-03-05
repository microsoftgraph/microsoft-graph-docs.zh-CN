---
title: 获取 groupPolicyMigrationReport
description: 读取 groupPolicyMigrationReport 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93eba94c40126f8e4e37394b626f38030c994db0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465469"
---
# <a name="get-grouppolicymigrationreport"></a><span data-ttu-id="e00f4-103">获取 groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="e00f4-103">Get groupPolicyMigrationReport</span></span>

<span data-ttu-id="e00f4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e00f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e00f4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e00f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e00f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e00f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e00f4-107">读取[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e00f4-107">Read properties and relationships of the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e00f4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e00f4-108">Prerequisites</span></span>
<span data-ttu-id="e00f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e00f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e00f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e00f4-111">Permission type</span></span>|<span data-ttu-id="e00f4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e00f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e00f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e00f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e00f4-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e00f4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e00f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e00f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e00f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e00f4-116">Not supported.</span></span>|
|<span data-ttu-id="e00f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e00f4-117">Application</span></span>|<span data-ttu-id="e00f4-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e00f4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e00f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e00f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e00f4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e00f4-120">Optional query parameters</span></span>
<span data-ttu-id="e00f4-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e00f4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e00f4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e00f4-122">Request headers</span></span>
|<span data-ttu-id="e00f4-123">标头</span><span class="sxs-lookup"><span data-stu-id="e00f4-123">Header</span></span>|<span data-ttu-id="e00f4-124">值</span><span class="sxs-lookup"><span data-stu-id="e00f4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e00f4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e00f4-125">Authorization</span></span>|<span data-ttu-id="e00f4-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e00f4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e00f4-127">接受</span><span class="sxs-lookup"><span data-stu-id="e00f4-127">Accept</span></span>|<span data-ttu-id="e00f4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e00f4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e00f4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e00f4-129">Request body</span></span>
<span data-ttu-id="e00f4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e00f4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e00f4-131">响应</span><span class="sxs-lookup"><span data-stu-id="e00f4-131">Response</span></span>
<span data-ttu-id="e00f4-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e00f4-132">If successful, this method returns a `200 OK` response code and [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e00f4-133">示例</span><span class="sxs-lookup"><span data-stu-id="e00f4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e00f4-134">请求</span><span class="sxs-lookup"><span data-stu-id="e00f4-134">Request</span></span>
<span data-ttu-id="e00f4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e00f4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

### <a name="response"></a><span data-ttu-id="e00f4-136">响应</span><span class="sxs-lookup"><span data-stu-id="e00f4-136">Response</span></span>
<span data-ttu-id="e00f4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e00f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
    "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
    "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
    "displayName": "Display Name value",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
    "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
    "migrationReadiness": "partial",
    "targetedInActiveDirectory": true,
    "totalSettingsCount": 2,
    "supportedSettingsCount": 6,
    "supportedSettingsPercent": 8
  }
}
```





