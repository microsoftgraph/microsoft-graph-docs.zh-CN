---
title: 获取 serviceUpdateMessage
description: 检索 serviceUpdateMessage 对象的属性和关系。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 63a9342d7c1db2f8716d5f4e255e91630287ba1f
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151732"
---
# <a name="get-serviceupdatemessage"></a><span data-ttu-id="abb42-103">获取 serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="abb42-103">Get serviceUpdateMessage</span></span>
<span data-ttu-id="abb42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abb42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb42-105">检索 [serviceUpdateMessage 对象的属性和](../resources/serviceupdatemessage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="abb42-105">Retrieve the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.</span></span>

<span data-ttu-id="abb42-106">此操作检索租户的指定服务更新消息。</span><span class="sxs-lookup"><span data-stu-id="abb42-106">This operation retrieves a specified service update message for the tenant.</span></span> <span data-ttu-id="abb42-107">如果租户不存在消息，则操作将返回错误。</span><span class="sxs-lookup"><span data-stu-id="abb42-107">The operation returns an error if the message does not exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="abb42-108">权限</span><span class="sxs-lookup"><span data-stu-id="abb42-108">Permissions</span></span>
<span data-ttu-id="abb42-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abb42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb42-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="abb42-111">Permission type</span></span>|<span data-ttu-id="abb42-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abb42-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb42-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abb42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abb42-114">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb42-114">ServiceMessage.Read.All</span></span>|
|<span data-ttu-id="abb42-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abb42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb42-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="abb42-116">Not supported.</span></span>|
|<span data-ttu-id="abb42-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="abb42-117">Application</span></span>|<span data-ttu-id="abb42-118">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb42-118">ServiceMessage.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb42-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abb42-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abb42-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="abb42-120">Optional query parameters</span></span>
<span data-ttu-id="abb42-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="abb42-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abb42-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="abb42-122">Request headers</span></span>
|<span data-ttu-id="abb42-123">名称</span><span class="sxs-lookup"><span data-stu-id="abb42-123">Name</span></span>|<span data-ttu-id="abb42-124">说明</span><span class="sxs-lookup"><span data-stu-id="abb42-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abb42-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb42-125">Authorization</span></span>|<span data-ttu-id="abb42-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="abb42-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb42-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="abb42-128">Request body</span></span>
<span data-ttu-id="abb42-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="abb42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abb42-130">响应</span><span class="sxs-lookup"><span data-stu-id="abb42-130">Response</span></span>

<span data-ttu-id="abb42-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceUpdateMessage](../resources/serviceupdatemessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abb42-131">If successful, this method returns a `200 OK` response code and a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb42-132">示例</span><span class="sxs-lookup"><span data-stu-id="abb42-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="abb42-133">请求</span><span class="sxs-lookup"><span data-stu-id="abb42-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MC172851"],
  "name": "get_serviceupdatemessage"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC172851
```

### <a name="response"></a><span data-ttu-id="abb42-134">响应</span><span class="sxs-lookup"><span data-stu-id="abb42-134">Response</span></span>
><span data-ttu-id="abb42-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="abb42-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages/$entity",
    "startDateTime": "2019-02-01T18:51:00Z",
    "endDateTime": "2019-06-01T08:00:00Z",
    "lastModifiedDateTime": "2021-01-08T01:10:06.843Z",
    "title": "(Updated) New feature: Changes to PowerPoint and Word to open files faster",
    "id": "MC172851",
    "category": "StayInformed",
    "severity": "Normal",
    "tags": [
      "Updated message"
    ],
    "isMajorChange": true,
    "actionRequiredByDateTime": null,
    "services": [
      "SharePoint Online",
      "OneDrive for Business"
    ],
    "details": [
      {
        "name": "ExternalLink",
        "value": "https://support.office.com/article/office-document-cache-settings-4b497318-ae4f-4a99-be42-b242b2e8b692"
      }
    ],
    "body": {
      "contentType": "Text",
      "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout.  Thank you for your patience........"
    },
    "viewPoint": null
}
```