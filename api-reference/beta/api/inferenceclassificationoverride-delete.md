---
title: 删除 inferenceClassificationOverride
description: 删除由其 ID 指定的中心收件箱覆盖
localization_priority: Normal
ms.openlocfilehash: 7db351e11ccfa8e88fe97ff1ee22173a87242d57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870138"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="9f71f-103">删除 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9f71f-103">Delete inferenceClassificationOverride</span></span>

> <span data-ttu-id="9f71f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f71f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f71f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f71f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f71f-106">删除由其 ID 指定的[中心收件箱](../resources/manage-focused-inbox.md)覆盖</span><span class="sxs-lookup"><span data-stu-id="9f71f-106">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f71f-107">权限</span><span class="sxs-lookup"><span data-stu-id="9f71f-107">Permissions</span></span>
<span data-ttu-id="9f71f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f71f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f71f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f71f-110">Permission type</span></span>      | <span data-ttu-id="9f71f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f71f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f71f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f71f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f71f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f71f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f71f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f71f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f71f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f71f-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f71f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f71f-116">Application</span></span> | <span data-ttu-id="9f71f-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f71f-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f71f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f71f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9f71f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f71f-119">Request headers</span></span>
| <span data-ttu-id="9f71f-120">名称</span><span class="sxs-lookup"><span data-stu-id="9f71f-120">Name</span></span>       | <span data-ttu-id="9f71f-121">类型</span><span class="sxs-lookup"><span data-stu-id="9f71f-121">Type</span></span> | <span data-ttu-id="9f71f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9f71f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f71f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f71f-123">Authorization</span></span>  | <span data-ttu-id="9f71f-124">string</span><span class="sxs-lookup"><span data-stu-id="9f71f-124">string</span></span>  | <span data-ttu-id="9f71f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f71f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f71f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f71f-127">Request body</span></span>
<span data-ttu-id="9f71f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f71f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f71f-129">响应</span><span class="sxs-lookup"><span data-stu-id="9f71f-129">Response</span></span>

<span data-ttu-id="9f71f-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9f71f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f71f-132">示例</span><span class="sxs-lookup"><span data-stu-id="9f71f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f71f-133">请求</span><span class="sxs-lookup"><span data-stu-id="9f71f-133">Request</span></span>
<span data-ttu-id="9f71f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f71f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="9f71f-135">响应</span><span class="sxs-lookup"><span data-stu-id="9f71f-135">Response</span></span>
<span data-ttu-id="9f71f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f71f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
