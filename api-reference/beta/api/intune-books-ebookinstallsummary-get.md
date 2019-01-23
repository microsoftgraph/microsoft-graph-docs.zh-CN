---
title: 获取 eBookInstallSummary
description: 读取 eBookInstallSummary 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f1052183ac5a6fb0c097a3c4da7b6a7f1cd64af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396929"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="a453a-103">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a453a-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="a453a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a453a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a453a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a453a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a453a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a453a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a453a-107">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a453a-107">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a453a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a453a-108">Prerequisites</span></span>
<span data-ttu-id="a453a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a453a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a453a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a453a-111">Permission type</span></span>|<span data-ttu-id="a453a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a453a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a453a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a453a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a453a-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a453a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a453a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a453a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a453a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a453a-116">Not supported.</span></span>|
|<span data-ttu-id="a453a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a453a-117">Application</span></span>|<span data-ttu-id="a453a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a453a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a453a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a453a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a453a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a453a-120">Optional query parameters</span></span>
<span data-ttu-id="a453a-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a453a-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a453a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a453a-122">Request headers</span></span>
|<span data-ttu-id="a453a-123">标头</span><span class="sxs-lookup"><span data-stu-id="a453a-123">Header</span></span>|<span data-ttu-id="a453a-124">值</span><span class="sxs-lookup"><span data-stu-id="a453a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a453a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a453a-125">Authorization</span></span>|<span data-ttu-id="a453a-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a453a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a453a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a453a-127">Accept</span></span>|<span data-ttu-id="a453a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a453a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a453a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a453a-129">Request body</span></span>
<span data-ttu-id="a453a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a453a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a453a-131">响应</span><span class="sxs-lookup"><span data-stu-id="a453a-131">Response</span></span>
<span data-ttu-id="a453a-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a453a-132">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a453a-133">示例</span><span class="sxs-lookup"><span data-stu-id="a453a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a453a-134">请求</span><span class="sxs-lookup"><span data-stu-id="a453a-134">Request</span></span>
<span data-ttu-id="a453a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a453a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="a453a-136">响应</span><span class="sxs-lookup"><span data-stu-id="a453a-136">Response</span></span>
<span data-ttu-id="a453a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a453a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": {
    "@odata.type": "#microsoft.graph.eBookInstallSummary",
    "id": "9708ad78-ad78-9708-78ad-089778ad0897",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notInstalledUserCount": 5
  }
}
```




