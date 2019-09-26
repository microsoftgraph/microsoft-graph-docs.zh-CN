---
title: 列出 roleDefinitions
description: 列出 roleDefinition 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb350f04cb37b51acf3c39587346600bd15791a2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189310"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="bd84b-103">列出 roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="bd84b-103">List roleDefinitions</span></span>

> <span data-ttu-id="bd84b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd84b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd84b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd84b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd84b-106">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd84b-106">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd84b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd84b-107">Prerequisites</span></span>
<span data-ttu-id="bd84b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd84b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd84b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd84b-110">Permission type</span></span>|<span data-ttu-id="bd84b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd84b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd84b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd84b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd84b-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd84b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="bd84b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd84b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd84b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd84b-115">Not supported.</span></span>|
|<span data-ttu-id="bd84b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd84b-116">Application</span></span>|<span data-ttu-id="bd84b-117">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd84b-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd84b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd84b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="bd84b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd84b-119">Request headers</span></span>
|<span data-ttu-id="bd84b-120">标头</span><span class="sxs-lookup"><span data-stu-id="bd84b-120">Header</span></span>|<span data-ttu-id="bd84b-121">值</span><span class="sxs-lookup"><span data-stu-id="bd84b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd84b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd84b-122">Authorization</span></span>|<span data-ttu-id="bd84b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd84b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd84b-124">接受</span><span class="sxs-lookup"><span data-stu-id="bd84b-124">Accept</span></span>|<span data-ttu-id="bd84b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd84b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd84b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd84b-126">Request body</span></span>
<span data-ttu-id="bd84b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd84b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd84b-128">响应</span><span class="sxs-lookup"><span data-stu-id="bd84b-128">Response</span></span>
<span data-ttu-id="bd84b-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bd84b-129">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd84b-130">示例</span><span class="sxs-lookup"><span data-stu-id="bd84b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd84b-131">请求</span><span class="sxs-lookup"><span data-stu-id="bd84b-131">Request</span></span>
<span data-ttu-id="bd84b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd84b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="bd84b-133">响应</span><span class="sxs-lookup"><span data-stu-id="bd84b-133">Response</span></span>
<span data-ttu-id="bd84b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd84b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




