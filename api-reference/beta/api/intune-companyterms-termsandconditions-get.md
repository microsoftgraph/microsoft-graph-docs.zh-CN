---
title: 获取 termsAndConditions
description: 读取 termsAndConditions 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f741df8ff5e244f2c90e86d5cd50ed633dfcf08
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244008"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="27515-103">获取 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="27515-103">Get termsAndConditions</span></span>

<span data-ttu-id="27515-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27515-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27515-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27515-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27515-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27515-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27515-107">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27515-107">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27515-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27515-108">Prerequisites</span></span>
<span data-ttu-id="27515-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27515-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27515-111">Permission type</span></span>|<span data-ttu-id="27515-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27515-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27515-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27515-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27515-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="27515-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="27515-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27515-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27515-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27515-116">Not supported.</span></span>|
|<span data-ttu-id="27515-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="27515-117">Application</span></span>|<span data-ttu-id="27515-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="27515-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27515-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27515-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27515-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="27515-120">Optional query parameters</span></span>
<span data-ttu-id="27515-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="27515-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27515-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="27515-122">Request headers</span></span>
|<span data-ttu-id="27515-123">标头</span><span class="sxs-lookup"><span data-stu-id="27515-123">Header</span></span>|<span data-ttu-id="27515-124">值</span><span class="sxs-lookup"><span data-stu-id="27515-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27515-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="27515-125">Authorization</span></span>|<span data-ttu-id="27515-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27515-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27515-127">接受</span><span class="sxs-lookup"><span data-stu-id="27515-127">Accept</span></span>|<span data-ttu-id="27515-128">application/json</span><span class="sxs-lookup"><span data-stu-id="27515-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27515-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="27515-129">Request body</span></span>
<span data-ttu-id="27515-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27515-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27515-131">响应</span><span class="sxs-lookup"><span data-stu-id="27515-131">Response</span></span>
<span data-ttu-id="27515-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27515-132">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27515-133">示例</span><span class="sxs-lookup"><span data-stu-id="27515-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="27515-134">请求</span><span class="sxs-lookup"><span data-stu-id="27515-134">Request</span></span>
<span data-ttu-id="27515-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27515-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="27515-136">响应</span><span class="sxs-lookup"><span data-stu-id="27515-136">Response</span></span>
<span data-ttu-id="27515-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27515-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




