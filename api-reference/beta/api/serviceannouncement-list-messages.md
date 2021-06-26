---
title: 列出邮件
description: 从 messages 导航属性中检索 serviceUpdateMessage 资源。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 9aca8752be18bad686677c4c718492ea93ccf0f4
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151452"
---
# <a name="list-messages"></a><span data-ttu-id="79a11-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="79a11-103">List messages</span></span>
<span data-ttu-id="79a11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79a11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79a11-105">从[messages 导航属性中检索 serviceUpdateMessage](../resources/serviceupdatemessage.md)资源。 </span><span class="sxs-lookup"><span data-stu-id="79a11-105">Retrieve the [serviceUpdateMessage](../resources/serviceupdatemessage.md) resources from the **messages** navigation property.</span></span>

<span data-ttu-id="79a11-106">此操作检索租户存在的所有服务更新消息。</span><span class="sxs-lookup"><span data-stu-id="79a11-106">This operation retrieves all service update messages that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="79a11-107">权限</span><span class="sxs-lookup"><span data-stu-id="79a11-107">Permissions</span></span>
<span data-ttu-id="79a11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79a11-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79a11-110">Permission type</span></span>|<span data-ttu-id="79a11-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79a11-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79a11-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79a11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79a11-113">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="79a11-113">ServiceMessage.Read.All</span></span>|
|<span data-ttu-id="79a11-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79a11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79a11-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79a11-115">Not supported.</span></span>|
|<span data-ttu-id="79a11-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79a11-116">Application</span></span>|<span data-ttu-id="79a11-117">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="79a11-117">ServiceMessage.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79a11-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79a11-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79a11-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="79a11-119">Optional query parameters</span></span>
<span data-ttu-id="79a11-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="79a11-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79a11-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="79a11-121">Request headers</span></span>
|<span data-ttu-id="79a11-122">名称</span><span class="sxs-lookup"><span data-stu-id="79a11-122">Name</span></span>|<span data-ttu-id="79a11-123">说明</span><span class="sxs-lookup"><span data-stu-id="79a11-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79a11-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79a11-124">Authorization</span></span>|<span data-ttu-id="79a11-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79a11-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79a11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79a11-127">Request body</span></span>
<span data-ttu-id="79a11-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79a11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79a11-129">响应</span><span class="sxs-lookup"><span data-stu-id="79a11-129">Response</span></span>

<span data-ttu-id="79a11-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceUpdateMessage](../resources/serviceupdatemessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="79a11-130">If successful, this method returns a `200 OK` response code and a collection of [serviceUpdateMessage](../resources/serviceupdatemessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79a11-131">示例</span><span class="sxs-lookup"><span data-stu-id="79a11-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="79a11-132">请求</span><span class="sxs-lookup"><span data-stu-id="79a11-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_serviceupdatemessage"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages
```

### <a name="response"></a><span data-ttu-id="79a11-133">响应</span><span class="sxs-lookup"><span data-stu-id="79a11-133">Response</span></span>
><span data-ttu-id="79a11-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79a11-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages",
  "value": [
    {
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
        "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout......"
      },
      "viewPoint": null
    }
  ]
}
```

