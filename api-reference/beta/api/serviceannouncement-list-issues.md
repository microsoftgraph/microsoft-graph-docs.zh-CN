---
title: 列出问题
description: 从 issues 导航属性检索 serviceHealthIssue 资源。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 5f3580d769c191def7145a363a0cf00e034b9fa3
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151445"
---
# <a name="list-issues"></a><span data-ttu-id="c1c60-103">列出问题</span><span class="sxs-lookup"><span data-stu-id="c1c60-103">List issues</span></span>
<span data-ttu-id="c1c60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1c60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c60-105">从 issues 导航属性中检索[serviceHealthIssue](../resources/servicehealthissue.md)资源。 </span><span class="sxs-lookup"><span data-stu-id="c1c60-105">Retrieve [serviceHealthIssue](../resources/servicehealthissue.md) resources from the **issues** navigation property.</span></span>

<span data-ttu-id="c1c60-106">此操作检索有关租户存在的所有服务运行状况问题的信息。</span><span class="sxs-lookup"><span data-stu-id="c1c60-106">This operation retrieves information about all service health issues that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1c60-107">权限</span><span class="sxs-lookup"><span data-stu-id="c1c60-107">Permissions</span></span>
<span data-ttu-id="c1c60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1c60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c60-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1c60-110">Permission type</span></span>|<span data-ttu-id="c1c60-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1c60-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1c60-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1c60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1c60-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1c60-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="c1c60-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1c60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1c60-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1c60-115">Not supported.</span></span>|
|<span data-ttu-id="c1c60-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1c60-116">Application</span></span>|<span data-ttu-id="c1c60-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1c60-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1c60-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1c60-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1c60-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1c60-119">Optional query parameters</span></span>
<span data-ttu-id="c1c60-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1c60-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1c60-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1c60-121">Request headers</span></span>
|<span data-ttu-id="c1c60-122">名称</span><span class="sxs-lookup"><span data-stu-id="c1c60-122">Name</span></span>|<span data-ttu-id="c1c60-123">说明</span><span class="sxs-lookup"><span data-stu-id="c1c60-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c1c60-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c60-124">Authorization</span></span>|<span data-ttu-id="c1c60-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1c60-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1c60-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1c60-127">Request body</span></span>
<span data-ttu-id="c1c60-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1c60-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1c60-129">响应</span><span class="sxs-lookup"><span data-stu-id="c1c60-129">Response</span></span>

<span data-ttu-id="c1c60-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceHealthIssue](../resources/servicehealthissue.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1c60-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealthIssue](../resources/servicehealthissue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1c60-131">示例</span><span class="sxs-lookup"><span data-stu-id="c1c60-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1c60-132">请求</span><span class="sxs-lookup"><span data-stu-id="c1c60-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues
```


### <a name="response"></a><span data-ttu-id="c1c60-133">响应</span><span class="sxs-lookup"><span data-stu-id="c1c60-133">Response</span></span>
><span data-ttu-id="c1c60-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1c60-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

