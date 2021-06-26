---
title: 获取 serviceHealthIssue
description: 检索 serviceHealthIssue 对象的属性和关系。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 2943c387085ded07745d8f781f496798a65ec3a6
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151431"
---
# <a name="get-servicehealthissue"></a><span data-ttu-id="23e23-103">获取 serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="23e23-103">Get serviceHealthIssue</span></span>
<span data-ttu-id="23e23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23e23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e23-105">检索 [serviceHealthIssue](../resources/servicehealthissue.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23e23-105">Retrieve the properties and relationships of a [serviceHealthIssue](../resources/servicehealthissue.md) object.</span></span>

<span data-ttu-id="23e23-106">此操作检索租户的指定服务运行状况问题。</span><span class="sxs-lookup"><span data-stu-id="23e23-106">This operation retrieves a specified service health issue for tenant.</span></span> <span data-ttu-id="23e23-107">如果租户不存在该问题，则操作将返回错误。</span><span class="sxs-lookup"><span data-stu-id="23e23-107">The operation returns an error if the issue does not exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="23e23-108">权限</span><span class="sxs-lookup"><span data-stu-id="23e23-108">Permissions</span></span>
<span data-ttu-id="23e23-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23e23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23e23-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="23e23-111">Permission type</span></span>|<span data-ttu-id="23e23-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23e23-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23e23-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23e23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23e23-114">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="23e23-114">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="23e23-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23e23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23e23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="23e23-116">Not supported.</span></span>|
|<span data-ttu-id="23e23-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="23e23-117">Application</span></span>|<span data-ttu-id="23e23-118">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="23e23-118">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e23-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23e23-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23e23-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23e23-120">Optional query parameters</span></span>
<span data-ttu-id="23e23-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23e23-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23e23-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="23e23-122">Request headers</span></span>
|<span data-ttu-id="23e23-123">名称</span><span class="sxs-lookup"><span data-stu-id="23e23-123">Name</span></span>|<span data-ttu-id="23e23-124">说明</span><span class="sxs-lookup"><span data-stu-id="23e23-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23e23-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="23e23-125">Authorization</span></span>|<span data-ttu-id="23e23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23e23-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23e23-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="23e23-128">Request body</span></span>
<span data-ttu-id="23e23-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23e23-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23e23-130">响应</span><span class="sxs-lookup"><span data-stu-id="23e23-130">Response</span></span>

<span data-ttu-id="23e23-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceHealthIssue](../resources/servicehealthissue.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23e23-131">If successful, this method returns a `200 OK` response code and a [serviceHealthIssue](../resources/servicehealthissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e23-132">示例</span><span class="sxs-lookup"><span data-stu-id="23e23-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="23e23-133">请求</span><span class="sxs-lookup"><span data-stu-id="23e23-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO226784"],
  "name": "get_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO226784
```


### <a name="response"></a><span data-ttu-id="23e23-134">响应</span><span class="sxs-lookup"><span data-stu-id="23e23-134">Response</span></span>
><span data-ttu-id="23e23-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="23e23-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues/$entity",
  "startDateTime": "2020-11-14T08:15:00Z",
  "endDateTime": "2020-11-14T09:45:00Z",
  "lastModifiedDateTime": "2020-11-14T11:06:53.353Z",
  "title": "Intermittently unable to access some Microsoft 365 services",
  "id": "MO226784",
  "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
  "classification": "Advisory",
  "origin": "Microsoft",
  "status": "ServiceRestored",
  "service": "Microsoft 365 suite",
  "feature": "Access",
  "featureGroup": "Portal",
  "isResolved": true,
  "details": [],
  "posts": [
    {
      "createdDateTime": "2020-11-12T07:07:38.97Z",
      "postType": "Regular",
      "description": {
        "contentType": "Text",
        "content": "Title: Intermittently unable to invite partners to meetings using some Microsoft 365 services\n\nUser Impact: Users may have been intermittently unable to invite partners to meetings using some Microsoft 365 services."
      }
    }
  ]
}
```

