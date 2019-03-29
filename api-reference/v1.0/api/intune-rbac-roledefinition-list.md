---
title: 列出 roleDefinitions
description: 列出 roleDefinition 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4df05098fccbc74056a0e10516b573dfce0ca141
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976454"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="ac99e-103">列出 roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ac99e-103">List roleDefinitions</span></span>

> <span data-ttu-id="ac99e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac99e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac99e-105">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ac99e-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac99e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ac99e-106">Prerequisites</span></span>
<span data-ttu-id="ac99e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac99e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac99e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac99e-109">Permission type</span></span>|<span data-ttu-id="ac99e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ac99e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac99e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac99e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac99e-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac99e-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ac99e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac99e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac99e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac99e-114">Not supported.</span></span>|
|<span data-ttu-id="ac99e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac99e-115">Application</span></span>|<span data-ttu-id="ac99e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac99e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac99e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac99e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ac99e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac99e-118">Request headers</span></span>
|<span data-ttu-id="ac99e-119">标头</span><span class="sxs-lookup"><span data-stu-id="ac99e-119">Header</span></span>|<span data-ttu-id="ac99e-120">值</span><span class="sxs-lookup"><span data-stu-id="ac99e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac99e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac99e-121">Authorization</span></span>|<span data-ttu-id="ac99e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ac99e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac99e-123">接受</span><span class="sxs-lookup"><span data-stu-id="ac99e-123">Accept</span></span>|<span data-ttu-id="ac99e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ac99e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac99e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac99e-125">Request body</span></span>
<span data-ttu-id="ac99e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac99e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac99e-127">响应</span><span class="sxs-lookup"><span data-stu-id="ac99e-127">Response</span></span>
<span data-ttu-id="ac99e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac99e-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac99e-129">示例</span><span class="sxs-lookup"><span data-stu-id="ac99e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac99e-130">请求</span><span class="sxs-lookup"><span data-stu-id="ac99e-130">Request</span></span>
<span data-ttu-id="ac99e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac99e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="ac99e-132">响应</span><span class="sxs-lookup"><span data-stu-id="ac99e-132">Response</span></span>
<span data-ttu-id="ac99e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac99e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



