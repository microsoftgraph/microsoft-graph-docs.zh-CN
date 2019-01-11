---
title: 列出附件
description: 获取附件对象附加到 Outlook 任务的列表。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: c76a11b960b8c1bb30e943cdc59205d2e0c3d4d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818905"
---
# <a name="list-attachments"></a><span data-ttu-id="bcac1-103">列出附件</span><span class="sxs-lookup"><span data-stu-id="bcac1-103">List attachments</span></span>

> <span data-ttu-id="bcac1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bcac1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcac1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bcac1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bcac1-106">获取[附件](../resources/attachment.md)对象附加到 Outlook 任务的列表。</span><span class="sxs-lookup"><span data-stu-id="bcac1-106">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcac1-107">权限</span><span class="sxs-lookup"><span data-stu-id="bcac1-107">Permissions</span></span>

<span data-ttu-id="bcac1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcac1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcac1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcac1-110">Permission type</span></span>      | <span data-ttu-id="bcac1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcac1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcac1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcac1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bcac1-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bcac1-113">Tasks.Read</span></span>    |
|<span data-ttu-id="bcac1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcac1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcac1-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bcac1-115">Tasks.Read</span></span>    |
|<span data-ttu-id="bcac1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcac1-116">Application</span></span> | <span data-ttu-id="bcac1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcac1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcac1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcac1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcac1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bcac1-119">Optional query parameters</span></span>

<span data-ttu-id="bcac1-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bcac1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcac1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcac1-121">Request headers</span></span>

| <span data-ttu-id="bcac1-122">名称</span><span class="sxs-lookup"><span data-stu-id="bcac1-122">Name</span></span>      |<span data-ttu-id="bcac1-123">说明</span><span class="sxs-lookup"><span data-stu-id="bcac1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bcac1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcac1-124">Authorization</span></span>  | <span data-ttu-id="bcac1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bcac1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcac1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcac1-127">Request body</span></span>

<span data-ttu-id="bcac1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bcac1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcac1-129">响应</span><span class="sxs-lookup"><span data-stu-id="bcac1-129">Response</span></span>

<span data-ttu-id="bcac1-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[attachment](../resources/attachment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bcac1-130">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcac1-131">示例</span><span class="sxs-lookup"><span data-stu-id="bcac1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcac1-132">请求</span><span class="sxs-lookup"><span data-stu-id="bcac1-132">Request</span></span>

<span data-ttu-id="bcac1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcac1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="bcac1-134">响应</span><span class="sxs-lookup"><span data-stu-id="bcac1-134">Response</span></span>

<span data-ttu-id="bcac1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bcac1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
