---
title: 列出 cartToClassAssociations
description: 列出 cartToClassAssociation 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1001702f1411a46a133398a804f6acb80aa4f257
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220901"
---
# <a name="list-carttoclassassociations"></a><span data-ttu-id="e4f5a-103">列出 cartToClassAssociations</span><span class="sxs-lookup"><span data-stu-id="e4f5a-103">List cartToClassAssociations</span></span>

<span data-ttu-id="e4f5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4f5a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4f5a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4f5a-107">列出 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-107">List properties and relationships of the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4f5a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4f5a-108">Prerequisites</span></span>
<span data-ttu-id="e4f5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f5a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4f5a-111">Permission type</span></span>|<span data-ttu-id="e4f5a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4f5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4f5a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4f5a-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4f5a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4f5a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4f5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4f5a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-116">Not supported.</span></span>|
|<span data-ttu-id="e4f5a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4f5a-117">Application</span></span>|<span data-ttu-id="e4f5a-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4f5a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4f5a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4f5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="e4f5a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4f5a-120">Request headers</span></span>
|<span data-ttu-id="e4f5a-121">标头</span><span class="sxs-lookup"><span data-stu-id="e4f5a-121">Header</span></span>|<span data-ttu-id="e4f5a-122">值</span><span class="sxs-lookup"><span data-stu-id="e4f5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4f5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4f5a-123">Authorization</span></span>|<span data-ttu-id="e4f5a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4f5a-125">接受</span><span class="sxs-lookup"><span data-stu-id="e4f5a-125">Accept</span></span>|<span data-ttu-id="e4f5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4f5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4f5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4f5a-127">Request body</span></span>
<span data-ttu-id="e4f5a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4f5a-129">响应</span><span class="sxs-lookup"><span data-stu-id="e4f5a-129">Response</span></span>
<span data-ttu-id="e4f5a-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-130">If successful, this method returns a `200 OK` response code and a collection of [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4f5a-131">示例</span><span class="sxs-lookup"><span data-stu-id="e4f5a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4f5a-132">请求</span><span class="sxs-lookup"><span data-stu-id="e4f5a-132">Request</span></span>
<span data-ttu-id="e4f5a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
```

### <a name="response"></a><span data-ttu-id="e4f5a-134">响应</span><span class="sxs-lookup"><span data-stu-id="e4f5a-134">Response</span></span>
<span data-ttu-id="e4f5a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4f5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cartToClassAssociation",
      "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "deviceCartIds": [
        "Device Cart Ids value"
      ],
      "classroomIds": [
        "Classroom Ids value"
      ]
    }
  ]
}
```




