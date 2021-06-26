---
title: 列出 healthOverviews
description: 从 healthOverviews 导航属性中检索 serviceHealth 资源。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: ef00a4e08ae8ac63e1f9a1ab76d2f5a71f9a8937
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151711"
---
# <a name="list-healthoverviews"></a><span data-ttu-id="abb56-103">列出 healthOverviews</span><span class="sxs-lookup"><span data-stu-id="abb56-103">List healthOverviews</span></span>
<span data-ttu-id="abb56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abb56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb56-105">从 **healthOverviews** 导航属性中检索 [serviceHealth](../resources/servicehealth.md)资源。</span><span class="sxs-lookup"><span data-stu-id="abb56-105">Retrieve the [serviceHealth](../resources/servicehealth.md) resources from the **healthOverviews** navigation property.</span></span>

<span data-ttu-id="abb56-106">此操作提供租户的所有订阅服务的运行状况报告。</span><span class="sxs-lookup"><span data-stu-id="abb56-106">This operation provides the health report of all subscribed services for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="abb56-107">权限</span><span class="sxs-lookup"><span data-stu-id="abb56-107">Permissions</span></span>
<span data-ttu-id="abb56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abb56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb56-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb56-110">Permission type</span></span>|<span data-ttu-id="abb56-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abb56-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb56-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abb56-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb56-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="abb56-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb56-115">Not supported.</span></span>|
|<span data-ttu-id="abb56-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb56-116">Application</span></span>|<span data-ttu-id="abb56-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb56-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb56-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb56-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/healthOverviews
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abb56-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="abb56-119">Optional query parameters</span></span>
<span data-ttu-id="abb56-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="abb56-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abb56-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb56-121">Request headers</span></span>
|<span data-ttu-id="abb56-122">名称</span><span class="sxs-lookup"><span data-stu-id="abb56-122">Name</span></span>|<span data-ttu-id="abb56-123">说明</span><span class="sxs-lookup"><span data-stu-id="abb56-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abb56-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb56-124">Authorization</span></span>|<span data-ttu-id="abb56-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="abb56-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb56-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb56-127">Request body</span></span>
<span data-ttu-id="abb56-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="abb56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abb56-129">响应</span><span class="sxs-lookup"><span data-stu-id="abb56-129">Response</span></span>

<span data-ttu-id="abb56-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceHealth](../resources/servicehealth.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="abb56-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealth](../resources/servicehealth.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abb56-131">示例</span><span class="sxs-lookup"><span data-stu-id="abb56-131">Examples</span></span>

### <a name="example-1-get-servicehealth-resources"></a><span data-ttu-id="abb56-132">示例 1：获取 serviceHealth 资源</span><span class="sxs-lookup"><span data-stu-id="abb56-132">Example 1: Get serviceHealth resources</span></span>

#### <a name="request"></a><span data-ttu-id="abb56-133">请求</span><span class="sxs-lookup"><span data-stu-id="abb56-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews
```

#### <a name="response"></a><span data-ttu-id="abb56-134">响应</span><span class="sxs-lookup"><span data-stu-id="abb56-134">Response</span></span>
><span data-ttu-id="abb56-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="abb56-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews",
  "value": [
    {
        "service": "Exchange Online",
        "status": "ServicaOperational",
        "id": "Exchange"
    },
    {
        "service": "Identity Service",
        "status": "ServiceRestored",
        "id": "OrgLiveID"
    },
    {
        "service": "Microsoft 365 suite",
        "status": "ServiceOperational",
        "id": "OSDPPlatform"
    }
  ]
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="abb56-136">示例 2：包含导航属性问题</span><span class="sxs-lookup"><span data-stu-id="abb56-136">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="abb56-137">请求</span><span class="sxs-lookup"><span data-stu-id="abb56-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews?$expand=issues
```

#### <a name="response"></a><span data-ttu-id="abb56-138">响应</span><span class="sxs-lookup"><span data-stu-id="abb56-138">Response</span></span>
><span data-ttu-id="abb56-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="abb56-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())",
  "value": [
    {
      "service": "Exchange Online",
      "status": "ServiceOperational",
      "id": "Exchange",
      "issues": [
          {
              "startDateTime": "2020-11-04T00:00:00Z",
              "endDateTime": "2020-11-20T17:00:00Z",
              "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
              "title": "Admins are unable to migrate some user mailboxes from IMAP using the Exchange admin center or PowerShell",
              "id": "EX226574",
              "impactDescription": "Admins attempting to migrate some user mailboxes using the Exchange admin center or PowerShell experienced failures.",
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
                        "content": "Title: Exchange Online service has login issue. We'll provide an update within 30 minutes."
                    }
                  }
                ]
          }
        ]
    }
  ]
}
```
