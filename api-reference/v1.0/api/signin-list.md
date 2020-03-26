---
title: 列出 signIn
description: 介绍 Microsoft Graph API 中登录资源（实体）的列表方法。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d7e76a44d060db5648bf8cb7af85e6b1cdc1185f
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948399"
---
# <a name="list-signins"></a><span data-ttu-id="3dd65-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="3dd65-103">List signIns</span></span>

<span data-ttu-id="3dd65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dd65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3dd65-105">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="3dd65-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="3dd65-106">在性质（用户名/密码作为身份验证令牌的一部分传递）和成功的联合登录中当前包括在登录日志中的登录登录。</span><span class="sxs-lookup"><span data-stu-id="3dd65-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dd65-107">权限</span><span class="sxs-lookup"><span data-stu-id="3dd65-107">Permissions</span></span>

<span data-ttu-id="3dd65-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="3dd65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="3dd65-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dd65-110">Permission type</span></span>      | <span data-ttu-id="3dd65-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dd65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dd65-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dd65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3dd65-113">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="3dd65-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="3dd65-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dd65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dd65-115">不支持</span><span class="sxs-lookup"><span data-stu-id="3dd65-115">Not supported</span></span>   |
|<span data-ttu-id="3dd65-116">应用</span><span class="sxs-lookup"><span data-stu-id="3dd65-116">Application</span></span> | <span data-ttu-id="3dd65-117">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="3dd65-117">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3dd65-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dd65-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3dd65-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3dd65-119">Optional query parameters</span></span>

<span data-ttu-id="3dd65-120">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3dd65-120">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="3dd65-121">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="3dd65-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="3dd65-122">名称</span><span class="sxs-lookup"><span data-stu-id="3dd65-122">Name</span></span>     |<span data-ttu-id="3dd65-123">说明</span><span class="sxs-lookup"><span data-stu-id="3dd65-123">Description</span></span>                            |<span data-ttu-id="3dd65-124">示例</span><span class="sxs-lookup"><span data-stu-id="3dd65-124">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="3dd65-125">$filter</span><span class="sxs-lookup"><span data-stu-id="3dd65-125">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="3dd65-126">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="3dd65-126">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="3dd65-127">$top</span><span class="sxs-lookup"><span data-stu-id="3dd65-127">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="3dd65-128">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="3dd65-128">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="3dd65-129">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="3dd65-129">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="3dd65-130">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="3dd65-130">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="3dd65-131">$filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="3dd65-131">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="3dd65-132">属性名</span><span class="sxs-lookup"><span data-stu-id="3dd65-132">Attribute name</span></span> |<span data-ttu-id="3dd65-133">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="3dd65-133">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="3dd65-134">id</span><span class="sxs-lookup"><span data-stu-id="3dd65-134">id</span></span>|<span data-ttu-id="3dd65-135">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-135">eq</span></span>|
|<span data-ttu-id="3dd65-136">userId</span><span class="sxs-lookup"><span data-stu-id="3dd65-136">userId</span></span>|<span data-ttu-id="3dd65-137">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-137">eq</span></span>|
|<span data-ttu-id="3dd65-138">appId</span><span class="sxs-lookup"><span data-stu-id="3dd65-138">appId</span></span>|<span data-ttu-id="3dd65-139">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-139">eq</span></span>|
|<span data-ttu-id="3dd65-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dd65-140">createdDateTime</span></span>| <span data-ttu-id="3dd65-141">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="3dd65-141">eq, le, ge</span></span>|
|<span data-ttu-id="3dd65-142">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3dd65-142">userDisplayName</span></span>| <span data-ttu-id="3dd65-143">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-143">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3dd65-144">userPrincipalName</span></span>| <span data-ttu-id="3dd65-145">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-145">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3dd65-146">appDisplayName</span></span>| <span data-ttu-id="3dd65-147">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-147">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-148">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3dd65-148">ipAddress</span></span>| <span data-ttu-id="3dd65-149">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-149">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-150">location/city</span><span class="sxs-lookup"><span data-stu-id="3dd65-150">location/city</span></span>| <span data-ttu-id="3dd65-151">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-151">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-152">location/state</span><span class="sxs-lookup"><span data-stu-id="3dd65-152">location/state</span></span>| <span data-ttu-id="3dd65-153">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-153">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-154">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3dd65-154">location/countryOrRegion</span></span>| <span data-ttu-id="3dd65-155">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-155">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-156">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="3dd65-156">status/errorCode</span></span>|<span data-ttu-id="3dd65-157">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-157">eq</span></span>|
|<span data-ttu-id="3dd65-158">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="3dd65-158">initiatedBy/user/id</span></span>|<span data-ttu-id="3dd65-159">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-159">eq</span></span>|
|<span data-ttu-id="3dd65-160">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="3dd65-160">initiatedBy/user/displayName</span></span>| <span data-ttu-id="3dd65-161">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-161">eq</span></span>|
|<span data-ttu-id="3dd65-162">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3dd65-162">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="3dd65-163">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-163">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-164">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="3dd65-164">clientAppUsed</span></span>| <span data-ttu-id="3dd65-165">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-165">eq</span></span>|
|<span data-ttu-id="3dd65-166">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="3dd65-166">conditionalAccessStatus</span></span> | <span data-ttu-id="3dd65-167">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-167">eq</span></span>|
|<span data-ttu-id="3dd65-168">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="3dd65-168">deviceDetail/browser</span></span>| <span data-ttu-id="3dd65-169">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-169">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-170">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3dd65-170">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="3dd65-171">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="3dd65-171">eq, startswith</span></span>|
|<span data-ttu-id="3dd65-172">correlationId</span><span class="sxs-lookup"><span data-stu-id="3dd65-172">correlationId</span></span>| <span data-ttu-id="3dd65-173">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-173">eq</span></span>|
|<span data-ttu-id="3dd65-174">isRisky</span><span class="sxs-lookup"><span data-stu-id="3dd65-174">isRisky</span></span>| <span data-ttu-id="3dd65-175">eq</span><span class="sxs-lookup"><span data-stu-id="3dd65-175">eq</span></span>|

## <a name="response"></a><span data-ttu-id="3dd65-176">响应</span><span class="sxs-lookup"><span data-stu-id="3dd65-176">Response</span></span>

<span data-ttu-id="3dd65-177">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3dd65-177">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dd65-178">示例</span><span class="sxs-lookup"><span data-stu-id="3dd65-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dd65-179">请求</span><span class="sxs-lookup"><span data-stu-id="3dd65-179">Request</span></span>

<span data-ttu-id="3dd65-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dd65-180">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3dd65-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dd65-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="3dd65-182">C#</span><span class="sxs-lookup"><span data-stu-id="3dd65-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dd65-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dd65-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dd65-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dd65-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dd65-185">Java</span><span class="sxs-lookup"><span data-stu-id="3dd65-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3dd65-186">响应</span><span class="sxs-lookup"><span data-stu-id="3dd65-186">Response</span></span>

<span data-ttu-id="3dd65-187">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3dd65-187">Here is an example of the response.</span></span>
><span data-ttu-id="3dd65-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3dd65-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signIns?$top=1&$skiptoken=9177f2e3532fcd4c4d225f68f7b9bdf7_1",
    "value": [
        {
            "id": "66ea54eb-6301-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test Contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-ae82-4189-b4e2-a37c6808512d",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "correlationId": "d79f5bee-5860-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "isInteractive": true,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
              ]
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
