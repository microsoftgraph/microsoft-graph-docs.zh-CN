---
title: 获取 serviceHealth
description: 检索 serviceHealth 对象的属性和关系。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 97ad1e2065c8d117e9532213ff192c78467adb7d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210739"
---
# <a name="get-servicehealth"></a><span data-ttu-id="36c7a-103">获取 serviceHealth</span><span class="sxs-lookup"><span data-stu-id="36c7a-103">Get serviceHealth</span></span>
<span data-ttu-id="36c7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36c7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36c7a-105">检索 [serviceHealth 对象的属性和](../resources/servicehealth.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="36c7a-105">Retrieve the properties and relationships of a [serviceHealth](../resources/servicehealth.md) object.</span></span>

<span data-ttu-id="36c7a-106">此操作为租户提供指定服务的运行状况信息。</span><span class="sxs-lookup"><span data-stu-id="36c7a-106">This operation provides the health information of a specified service for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="36c7a-107">权限</span><span class="sxs-lookup"><span data-stu-id="36c7a-107">Permissions</span></span>
<span data-ttu-id="36c7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36c7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c7a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36c7a-110">Permission type</span></span>|<span data-ttu-id="36c7a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36c7a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36c7a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36c7a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36c7a-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="36c7a-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="36c7a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36c7a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36c7a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36c7a-115">Not supported.</span></span>|
|<span data-ttu-id="36c7a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36c7a-116">Application</span></span>|<span data-ttu-id="36c7a-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="36c7a-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36c7a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36c7a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /admin/serviceAnnouncement/healthOverviews/{ServiceName}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36c7a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36c7a-119">Optional query parameters</span></span>
<span data-ttu-id="36c7a-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36c7a-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36c7a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="36c7a-121">Request headers</span></span>
|<span data-ttu-id="36c7a-122">名称</span><span class="sxs-lookup"><span data-stu-id="36c7a-122">Name</span></span>|<span data-ttu-id="36c7a-123">说明</span><span class="sxs-lookup"><span data-stu-id="36c7a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="36c7a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c7a-124">Authorization</span></span>|<span data-ttu-id="36c7a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36c7a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36c7a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36c7a-127">Request body</span></span>
<span data-ttu-id="36c7a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36c7a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c7a-129">响应</span><span class="sxs-lookup"><span data-stu-id="36c7a-129">Response</span></span>

<span data-ttu-id="36c7a-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [serviceHealth](../resources/servicehealth.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36c7a-130">If successful, this method returns a `200 OK` response code and a [serviceHealth](../resources/servicehealth.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36c7a-131">示例</span><span class="sxs-lookup"><span data-stu-id="36c7a-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-servicehealth-object"></a><span data-ttu-id="36c7a-132">示例 1：获取 serviceHealth 对象的属性</span><span class="sxs-lookup"><span data-stu-id="36c7a-132">Example 1: Get the properties of a serviceHealth object</span></span>

#### <a name="request"></a><span data-ttu-id="36c7a-133">请求</span><span class="sxs-lookup"><span data-stu-id="36c7a-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="36c7a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="36c7a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite
```
# <a name="c"></a>[<span data-ttu-id="36c7a-135">C#</span><span class="sxs-lookup"><span data-stu-id="36c7a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-servicehealth-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36c7a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36c7a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-servicehealth-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36c7a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36c7a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-servicehealth-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36c7a-138">Java</span><span class="sxs-lookup"><span data-stu-id="36c7a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-servicehealth-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36c7a-139">响应</span><span class="sxs-lookup"><span data-stu-id="36c7a-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews/$entity",
    "service": "Microsoft 365 suite",
    "status": "RestoringService",
    "id": "OSDPPlatform"
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="36c7a-140">示例 2：包含导航属性问题</span><span class="sxs-lookup"><span data-stu-id="36c7a-140">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="36c7a-141">请求</span><span class="sxs-lookup"><span data-stu-id="36c7a-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="36c7a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="36c7a-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite?$expand=issues
```
# <a name="c"></a>[<span data-ttu-id="36c7a-143">C#</span><span class="sxs-lookup"><span data-stu-id="36c7a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-servicehealth-with-issues-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36c7a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36c7a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-servicehealth-with-issues-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36c7a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36c7a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-servicehealth-with-issues-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36c7a-146">Java</span><span class="sxs-lookup"><span data-stu-id="36c7a-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-servicehealth-with-issues-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36c7a-147">响应</span><span class="sxs-lookup"><span data-stu-id="36c7a-147">Response</span></span>
><span data-ttu-id="36c7a-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36c7a-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())/$entity",
  "service": "Microsoft 365 suite",
  "status": "ServiceOperational",
  "id": "OSDPPlatform",
  "issues": [
        {
          "startDateTime": "2020-11-04T00:00:00Z",
          "endDateTime": "2020-11-20T17:00:00Z",
          "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
          "title": "Intermittently unable to access some Microsoft 365 services",
          "id": "MO226574",
          "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
          "classification": "Advisory",
          "origin": "Microsoft",
          "status": "ServiceRestored",
          "service": "Exchange Online",
          "feature": "Tenant Administration (Provisioning, Remote PowerShell)",
          "featureGroup": "Management and Provisioning",
          "isResolved": true,
          "details": [],
          "posts": [
              {
                "createdDateTime": "2020-11-12T07:07:38.97Z",
                "postType": "Regular",
                "description": {
                    "contentType": "Text",
                    "content": "Users may have been intermittently unable to access some Microsoft 365 services. We'll provide an update within 30 minutes."
                  }
              }
          ]
        }
    ]
}
```
