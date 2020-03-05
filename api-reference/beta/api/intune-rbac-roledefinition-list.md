---
title: 列出 roleDefinitions
description: 列出 roleDefinition 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab0df9a407715651ecb3c3ce567da3a428c81c50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459679"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="733a8-103">列出 roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="733a8-103">List roleDefinitions</span></span>

<span data-ttu-id="733a8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="733a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="733a8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="733a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="733a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="733a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="733a8-107">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="733a8-107">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="733a8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="733a8-108">Prerequisites</span></span>
<span data-ttu-id="733a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="733a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="733a8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="733a8-111">Permission type</span></span>|<span data-ttu-id="733a8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="733a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="733a8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="733a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="733a8-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="733a8-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="733a8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="733a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="733a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="733a8-116">Not supported.</span></span>|
|<span data-ttu-id="733a8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="733a8-117">Application</span></span>|<span data-ttu-id="733a8-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="733a8-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="733a8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="733a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="733a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="733a8-120">Request headers</span></span>
|<span data-ttu-id="733a8-121">标头</span><span class="sxs-lookup"><span data-stu-id="733a8-121">Header</span></span>|<span data-ttu-id="733a8-122">值</span><span class="sxs-lookup"><span data-stu-id="733a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="733a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="733a8-123">Authorization</span></span>|<span data-ttu-id="733a8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="733a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="733a8-125">接受</span><span class="sxs-lookup"><span data-stu-id="733a8-125">Accept</span></span>|<span data-ttu-id="733a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="733a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="733a8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="733a8-127">Request body</span></span>
<span data-ttu-id="733a8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="733a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="733a8-129">响应</span><span class="sxs-lookup"><span data-stu-id="733a8-129">Response</span></span>
<span data-ttu-id="733a8-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="733a8-130">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="733a8-131">示例</span><span class="sxs-lookup"><span data-stu-id="733a8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="733a8-132">请求</span><span class="sxs-lookup"><span data-stu-id="733a8-132">Request</span></span>
<span data-ttu-id="733a8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="733a8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="733a8-134">响应</span><span class="sxs-lookup"><span data-stu-id="733a8-134">Response</span></span>
<span data-ttu-id="733a8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="733a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1477

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleDefinition",
      "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
      "displayName": "Display Name value",
      "description": "Description value",
      "permissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
          "actions": [
            "Actions value"
          ],
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
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
          "actions": [
            "Actions value"
          ],
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
      "isBuiltInRoleDefinition": true,
      "isBuiltIn": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```





