---
title: 列出问题
description: 从 issues 导航属性检索 serviceHealthIssue 资源。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: b798ef786d4c90756d76c9980554cd569ae314c6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208888"
---
# <a name="list-issues"></a><span data-ttu-id="ef839-103">列出问题</span><span class="sxs-lookup"><span data-stu-id="ef839-103">List issues</span></span>
<span data-ttu-id="ef839-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef839-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef839-105">从 issues 导航属性中检索[serviceHealthIssue](../resources/servicehealthissue.md)资源。 </span><span class="sxs-lookup"><span data-stu-id="ef839-105">Retrieve [serviceHealthIssue](../resources/servicehealthissue.md) resources from the **issues** navigation property.</span></span>

<span data-ttu-id="ef839-106">此操作检索有关租户存在的所有服务运行状况问题的信息。</span><span class="sxs-lookup"><span data-stu-id="ef839-106">This operation retrieves information about all service health issues that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef839-107">权限</span><span class="sxs-lookup"><span data-stu-id="ef839-107">Permissions</span></span>
<span data-ttu-id="ef839-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef839-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef839-110">Permission type</span></span>|<span data-ttu-id="ef839-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef839-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef839-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef839-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef839-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef839-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="ef839-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef839-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef839-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef839-115">Not supported.</span></span>|
|<span data-ttu-id="ef839-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef839-116">Application</span></span>|<span data-ttu-id="ef839-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef839-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef839-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef839-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef839-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ef839-119">Optional query parameters</span></span>
<span data-ttu-id="ef839-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ef839-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef839-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef839-121">Request headers</span></span>
|<span data-ttu-id="ef839-122">名称</span><span class="sxs-lookup"><span data-stu-id="ef839-122">Name</span></span>|<span data-ttu-id="ef839-123">说明</span><span class="sxs-lookup"><span data-stu-id="ef839-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef839-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef839-124">Authorization</span></span>|<span data-ttu-id="ef839-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef839-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef839-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef839-127">Request body</span></span>
<span data-ttu-id="ef839-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef839-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef839-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef839-129">Response</span></span>

<span data-ttu-id="ef839-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceHealthIssue](../resources/servicehealthissue.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ef839-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealthIssue](../resources/servicehealthissue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef839-131">示例</span><span class="sxs-lookup"><span data-stu-id="ef839-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef839-132">请求</span><span class="sxs-lookup"><span data-stu-id="ef839-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef839-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef839-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues
```
# <a name="c"></a>[<span data-ttu-id="ef839-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef839-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-servicehealthissue-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef839-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef839-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-servicehealthissue-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef839-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef839-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-servicehealthissue-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef839-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef839-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-servicehealthissue-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ef839-138">响应</span><span class="sxs-lookup"><span data-stu-id="ef839-138">Response</span></span>
><span data-ttu-id="ef839-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ef839-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues",
  "value": [
    {
      "startDateTime": "2020-11-13T21:00:00Z",
      "endDateTime": "2020-11-14T17:15:00Z",
      "lastModifiedDateTime": "2020-11-14T18:20:24.767Z",
      "title": "Limited number of users unable to send or receive email through the Exchange Online service",
      "id": "EX226792",
      "impactDescription": "Users may have been unable to send or receive email through the Exchange Online service.",
      "classification": "Incident",
      "origin": "Microsoft",
      "status": "ServiceRestored",
      "service": "Exchange Online",
      "feature": "Mailflow - delayed delivery from Internet",
      "featureGroup": "E-Mail timely delivery",
      "isResolved": true,
      "details": [
        {
          "name": "NotifyInApp",
          "value": "True"
        }
      ],
      "posts": [
        {
          "createdDateTime": "2020-11-12T07:07:38.97Z",
          "postType": "Regular",
          "description": {
            "contentType": "Text",
            "content": "Title: Limited number of users unable to send or receive email through the Exchange Online service\n\nUser Impact: Users may be unable to send or receive email through the Exchange Online service."
          }
        }
      ]
    }
  ]
}
```

