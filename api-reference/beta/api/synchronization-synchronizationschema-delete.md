---
title: 删除 synchronizationSchema
description: 删除自定义的架构，并将架构重置为默认配置。 如果模板的上下文中删除架构，则它将重置架构为一个相关联的模板的默认`factoryTag`。
ms.openlocfilehash: 81c1a918b10e8f4553b3e99312f20bb538bfbe4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047485"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="7965a-104">删除 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="7965a-104">Delete synchronizationSchema</span></span>

> <span data-ttu-id="7965a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7965a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7965a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7965a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7965a-107">删除自定义的架构，并将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="7965a-107">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="7965a-108">如果模板的上下文中删除架构，则它将重置架构为一个相关联的模板的默认`factoryTag`。</span><span class="sxs-lookup"><span data-stu-id="7965a-108">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7965a-109">权限</span><span class="sxs-lookup"><span data-stu-id="7965a-109">Permissions</span></span>
<span data-ttu-id="7965a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7965a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7965a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7965a-112">Permission type</span></span>                        | <span data-ttu-id="7965a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7965a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7965a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7965a-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="7965a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7965a-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7965a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7965a-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7965a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7965a-117">Not supported.</span></span>|
|<span data-ttu-id="7965a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7965a-118">Application</span></span>                            |<span data-ttu-id="7965a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7965a-119">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="7965a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7965a-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="7965a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7965a-121">Request headers</span></span>

| <span data-ttu-id="7965a-122">名称</span><span class="sxs-lookup"><span data-stu-id="7965a-122">Name</span></span>           | <span data-ttu-id="7965a-123">类型</span><span class="sxs-lookup"><span data-stu-id="7965a-123">Type</span></span>    | <span data-ttu-id="7965a-124">说明</span><span class="sxs-lookup"><span data-stu-id="7965a-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7965a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7965a-125">Authorization</span></span>  | <span data-ttu-id="7965a-126">string</span><span class="sxs-lookup"><span data-stu-id="7965a-126">string</span></span>  | <span data-ttu-id="7965a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7965a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7965a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7965a-129">Request body</span></span>

<span data-ttu-id="7965a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7965a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7965a-131">响应</span><span class="sxs-lookup"><span data-stu-id="7965a-131">Response</span></span>

<span data-ttu-id="7965a-132">如果成功，此方法返回 `201 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7965a-132">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="7965a-133">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="7965a-133">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="7965a-134">示例</span><span class="sxs-lookup"><span data-stu-id="7965a-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7965a-135">请求</span><span class="sxs-lookup"><span data-stu-id="7965a-135">Request</span></span>
<span data-ttu-id="7965a-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7965a-136">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="7965a-137">响应</span><span class="sxs-lookup"><span data-stu-id="7965a-137">Response</span></span>
<span data-ttu-id="7965a-138">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="7965a-138">The following is an example of a response.</span></span>
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
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->