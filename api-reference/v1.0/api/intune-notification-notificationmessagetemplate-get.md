---
title: 获取 notificationMessageTemplate
description: 读取 notificationMessageTemplate 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13e5bf52bff2ff17e97cd8d82d04ae5512ea84fc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258714"
---
# <a name="get-notificationmessagetemplate"></a><span data-ttu-id="ffbae-103">获取 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ffbae-103">Get notificationMessageTemplate</span></span>

> <span data-ttu-id="ffbae-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffbae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffbae-105">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ffbae-105">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffbae-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffbae-106">Prerequisites</span></span>
<span data-ttu-id="ffbae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ffbae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ffbae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffbae-109">Permission type</span></span>|<span data-ttu-id="ffbae-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffbae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffbae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffbae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffbae-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffbae-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ffbae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffbae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffbae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffbae-114">Not supported.</span></span>|
|<span data-ttu-id="ffbae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffbae-115">Application</span></span>|<span data-ttu-id="ffbae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffbae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffbae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffbae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffbae-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ffbae-118">Optional query parameters</span></span>
<span data-ttu-id="ffbae-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ffbae-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffbae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffbae-120">Request headers</span></span>
|<span data-ttu-id="ffbae-121">标头</span><span class="sxs-lookup"><span data-stu-id="ffbae-121">Header</span></span>|<span data-ttu-id="ffbae-122">值</span><span class="sxs-lookup"><span data-stu-id="ffbae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffbae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffbae-123">Authorization</span></span>|<span data-ttu-id="ffbae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffbae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffbae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffbae-125">Accept</span></span>|<span data-ttu-id="ffbae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffbae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffbae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffbae-127">Request body</span></span>
<span data-ttu-id="ffbae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffbae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffbae-129">响应</span><span class="sxs-lookup"><span data-stu-id="ffbae-129">Response</span></span>
<span data-ttu-id="ffbae-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffbae-130">If successful, this method returns a `200 OK` response code and [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffbae-131">示例</span><span class="sxs-lookup"><span data-stu-id="ffbae-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffbae-132">请求</span><span class="sxs-lookup"><span data-stu-id="ffbae-132">Request</span></span>
<span data-ttu-id="ffbae-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffbae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="ffbae-134">响应</span><span class="sxs-lookup"><span data-stu-id="ffbae-134">Response</span></span>
<span data-ttu-id="ffbae-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffbae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.notificationMessageTemplate",
    "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "defaultLocale": "Default Locale value",
    "brandingOptions": "includeCompanyLogo"
  }
}
```



