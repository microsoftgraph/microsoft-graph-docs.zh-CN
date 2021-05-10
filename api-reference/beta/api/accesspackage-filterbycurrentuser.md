---
title: accessPackage： filterByCurrentUser
description: 检索在已登录用户上筛选的 accesspackage 对象列表。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a4212c06606c6363a31e64dee7da820d93ea13fa
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299139"
---
# <a name="accesspackage-filterbycurrentuser"></a><span data-ttu-id="5206b-103">accessPackage： filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="5206b-103">accessPackage: filterByCurrentUser</span></span>
<span data-ttu-id="5206b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5206b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5206b-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索已登录用户筛选的 [accessPackage](../resources/accesspackage.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="5206b-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackage](../resources/accesspackage.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5206b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5206b-106">Permissions</span></span>
<span data-ttu-id="5206b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5206b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5206b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5206b-109">Permission type</span></span>|<span data-ttu-id="5206b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5206b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5206b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5206b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5206b-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5206b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="5206b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5206b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5206b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5206b-114">Not supported.</span></span>|
|<span data-ttu-id="5206b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5206b-115">Application</span></span>|<span data-ttu-id="5206b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5206b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5206b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5206b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="5206b-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="5206b-118">Function parameters</span></span>
<span data-ttu-id="5206b-119">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="5206b-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5206b-120">参数</span><span class="sxs-lookup"><span data-stu-id="5206b-120">Parameter</span></span>|<span data-ttu-id="5206b-121">类型</span><span class="sxs-lookup"><span data-stu-id="5206b-121">Type</span></span>|<span data-ttu-id="5206b-122">说明</span><span class="sxs-lookup"><span data-stu-id="5206b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5206b-123">on</span><span class="sxs-lookup"><span data-stu-id="5206b-123">on</span></span>|[<span data-ttu-id="5206b-124">accessPackageFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="5206b-124">accessPackageFilterByCurrentUserOptions</span></span>](../resources/accesspackage-accesspackagefilterbycurrentuseroptions.md)|<span data-ttu-id="5206b-125">可用于在访问包列表上进行筛选的当前用户选项的列表。</span><span class="sxs-lookup"><span data-stu-id="5206b-125">The list of current user options that can be used to filter on the access packages list.</span></span>|

- <span data-ttu-id="5206b-126">`allowedRequestor` 用于获取允许登录用户提交访问 `accessPackage` 请求的对象。</span><span class="sxs-lookup"><span data-stu-id="5206b-126">`allowedRequestor` is used to get the `accessPackage` objects for which the signed-in user is allowed to submit access requests.</span></span> <span data-ttu-id="5206b-127">生成的列表包括调用方可以跨所有目录请求的所有访问包。</span><span class="sxs-lookup"><span data-stu-id="5206b-127">The resulting list includes all access packages that can be requested by the caller across all catalogs.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5206b-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="5206b-128">Request headers</span></span>
|<span data-ttu-id="5206b-129">名称</span><span class="sxs-lookup"><span data-stu-id="5206b-129">Name</span></span>|<span data-ttu-id="5206b-130">说明</span><span class="sxs-lookup"><span data-stu-id="5206b-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5206b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="5206b-131">Authorization</span></span>|<span data-ttu-id="5206b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5206b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5206b-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="5206b-134">Request body</span></span>
<span data-ttu-id="5206b-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5206b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5206b-136">响应</span><span class="sxs-lookup"><span data-stu-id="5206b-136">Response</span></span>

<span data-ttu-id="5206b-137">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 [accessPackage](../resources/accesspackage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5206b-137">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5206b-138">示例</span><span class="sxs-lookup"><span data-stu-id="5206b-138">Examples</span></span>
<span data-ttu-id="5206b-139">以下示例获取登录用户可以请求的访问包。</span><span class="sxs-lookup"><span data-stu-id="5206b-139">The following example gets the access packages that can be requested by the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="5206b-140">请求</span><span class="sxs-lookup"><span data-stu-id="5206b-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterByCurrentUser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')
```


### <a name="response"></a><span data-ttu-id="5206b-141">响应</span><span class="sxs-lookup"><span data-stu-id="5206b-141">Response</span></span>
> <span data-ttu-id="5206b-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5206b-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackage",
            "id": "d378b3b7-b42a-445a-8780-2841194f777e",
            "catalogId": "eb0f5e12-484d-4545-8ae1-fb1dfc28ab3c",
            "displayName": "Sales resources",
            "description": "Resources needed by the Sales department.",
            "isHidden": false,
            "isRoleScopesVisible": false,
            "createdBy": "TestGA@example.com",
            "createdDateTime": "2021-01-26T22:30:57.37Z",
            "modifiedBy": "TestGA@example.com",
            "modifiedDateTime": "2021-01-26T22:30:57.37Z"
        }
    ]
}
```

