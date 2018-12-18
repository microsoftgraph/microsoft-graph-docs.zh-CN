---
title: 列出 roleDefinitions
description: 列出 roleDefinition 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 2aa23644d075c03aeb5b19551672214f15e0f4bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319647"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="12ff6-103">列出 roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="12ff6-103">List roleDefinitions</span></span>

> <span data-ttu-id="12ff6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12ff6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12ff6-105">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12ff6-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12ff6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="12ff6-106">Prerequisites</span></span>
<span data-ttu-id="12ff6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="12ff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12ff6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12ff6-109">Permission type</span></span>|<span data-ttu-id="12ff6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12ff6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12ff6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12ff6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12ff6-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="12ff6-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="12ff6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12ff6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12ff6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12ff6-114">Not supported.</span></span>|
|<span data-ttu-id="12ff6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12ff6-115">Application</span></span>|<span data-ttu-id="12ff6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12ff6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12ff6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12ff6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="12ff6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="12ff6-118">Request headers</span></span>
|<span data-ttu-id="12ff6-119">标头</span><span class="sxs-lookup"><span data-stu-id="12ff6-119">Header</span></span>|<span data-ttu-id="12ff6-120">值</span><span class="sxs-lookup"><span data-stu-id="12ff6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12ff6-121">授权</span><span class="sxs-lookup"><span data-stu-id="12ff6-121">Authorization</span></span>|<span data-ttu-id="12ff6-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12ff6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12ff6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="12ff6-123">Accept</span></span>|<span data-ttu-id="12ff6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12ff6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12ff6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="12ff6-125">Request body</span></span>
<span data-ttu-id="12ff6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12ff6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12ff6-127">响应</span><span class="sxs-lookup"><span data-stu-id="12ff6-127">Response</span></span>
<span data-ttu-id="12ff6-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="12ff6-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12ff6-129">示例</span><span class="sxs-lookup"><span data-stu-id="12ff6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="12ff6-130">请求</span><span class="sxs-lookup"><span data-stu-id="12ff6-130">Request</span></span>
<span data-ttu-id="12ff6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12ff6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="12ff6-132">响应</span><span class="sxs-lookup"><span data-stu-id="12ff6-132">Response</span></span>
<span data-ttu-id="12ff6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12ff6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 746

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleDefinition",
      "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
      "displayName": "Display Name value",
      "description": "Description value",
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
          "resourceActions": [
            {
              "@odata.type": "microsoft.graph.resourceAction",
              "allowedResourceActions": [
                "Allowed Resource Actions value"
              ],
              "notAllowedResourceActions": [
                "Not Allowed Resource Actions value"
              ]
            }
          ]
        }
      ],
      "isBuiltIn": true
    }
  ]
}
```



