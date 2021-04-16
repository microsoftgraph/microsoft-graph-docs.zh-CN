---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 798fa1eb36a9f9dd58aae6cae8dd4e4960b6299c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864611"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="76ed2-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="76ed2-103">Get deviceAppManagement</span></span>

<span data-ttu-id="76ed2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76ed2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76ed2-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="76ed2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76ed2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76ed2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76ed2-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76ed2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76ed2-108">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76ed2-108">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76ed2-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="76ed2-109">Prerequisites</span></span>

<span data-ttu-id="76ed2-110">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="76ed2-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="76ed2-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76ed2-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="76ed2-112">请注意，相应的权限因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="76ed2-112">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="76ed2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="76ed2-113">Permission type</span></span>|<span data-ttu-id="76ed2-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76ed2-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="76ed2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76ed2-115">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="76ed2-116">&nbsp;&nbsp;**应用\*\*\*\*、书籍\*\*\*\*、载入**、**合作伙伴集成** 或 **策略集**</span><span class="sxs-lookup"><span data-stu-id="76ed2-116">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="76ed2-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="76ed2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="76ed2-118">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="76ed2-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="76ed2-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="76ed2-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="76ed2-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76ed2-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76ed2-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="76ed2-121">Not supported.</span></span>|
|<span data-ttu-id="76ed2-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="76ed2-122">Application</span></span>| |
| <span data-ttu-id="76ed2-123">&nbsp;&nbsp;**应用\*\*\*\*、书籍\*\*\*\*、载入**、**合作伙伴集成** 或 **策略集**</span><span class="sxs-lookup"><span data-stu-id="76ed2-123">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, **Partner Integration**, or **Policy Set**</span></span> | <span data-ttu-id="76ed2-124">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="76ed2-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="76ed2-125">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="76ed2-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="76ed2-126">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="76ed2-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76ed2-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76ed2-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76ed2-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76ed2-128">Optional query parameters</span></span>

<span data-ttu-id="76ed2-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76ed2-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76ed2-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="76ed2-130">Request headers</span></span>

|<span data-ttu-id="76ed2-131">标头</span><span class="sxs-lookup"><span data-stu-id="76ed2-131">Header</span></span>|<span data-ttu-id="76ed2-132">值</span><span class="sxs-lookup"><span data-stu-id="76ed2-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76ed2-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="76ed2-133">Authorization</span></span>|<span data-ttu-id="76ed2-134">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76ed2-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76ed2-135">接受</span><span class="sxs-lookup"><span data-stu-id="76ed2-135">Accept</span></span>|<span data-ttu-id="76ed2-136">application/json</span><span class="sxs-lookup"><span data-stu-id="76ed2-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76ed2-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="76ed2-137">Request body</span></span>

<span data-ttu-id="76ed2-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76ed2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76ed2-139">响应</span><span class="sxs-lookup"><span data-stu-id="76ed2-139">Response</span></span>

<span data-ttu-id="76ed2-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76ed2-140">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76ed2-141">示例</span><span class="sxs-lookup"><span data-stu-id="76ed2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="76ed2-142">请求</span><span class="sxs-lookup"><span data-stu-id="76ed2-142">Request</span></span>

<span data-ttu-id="76ed2-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76ed2-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="76ed2-144">响应</span><span class="sxs-lookup"><span data-stu-id="76ed2-144">Response</span></span>

<span data-ttu-id="76ed2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76ed2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```










