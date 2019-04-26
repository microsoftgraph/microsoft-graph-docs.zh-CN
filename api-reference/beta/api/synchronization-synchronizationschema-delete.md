---
title: 删除 synchronizationSchema
description: 删除自定义架构并将架构重置为默认配置。 如果在模板的上下文中删除了架构, 它会将架构重置为与模板关联的默认架构`factoryTag`。
localization_priority: Normal
ms.openlocfilehash: 0871de0ba5b48784e47fd5cc8d3ac890ab23748b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330611"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="e9f80-104">删除 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e9f80-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f80-105">删除自定义架构并将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="e9f80-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="e9f80-106">如果在模板的上下文中删除了架构, 它会将架构重置为与模板关联的默认架构`factoryTag`。</span><span class="sxs-lookup"><span data-stu-id="e9f80-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9f80-107">权限</span><span class="sxs-lookup"><span data-stu-id="e9f80-107">Permissions</span></span>
<span data-ttu-id="e9f80-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9f80-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9f80-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9f80-110">Permission type</span></span>                        | <span data-ttu-id="e9f80-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9f80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9f80-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9f80-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="e9f80-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9f80-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e9f80-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9f80-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e9f80-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9f80-115">Not supported.</span></span>|
|<span data-ttu-id="e9f80-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9f80-116">Application</span></span>                            |<span data-ttu-id="e9f80-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9f80-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e9f80-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9f80-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e9f80-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9f80-119">Request headers</span></span>

| <span data-ttu-id="e9f80-120">名称</span><span class="sxs-lookup"><span data-stu-id="e9f80-120">Name</span></span>           | <span data-ttu-id="e9f80-121">类型</span><span class="sxs-lookup"><span data-stu-id="e9f80-121">Type</span></span>    | <span data-ttu-id="e9f80-122">说明</span><span class="sxs-lookup"><span data-stu-id="e9f80-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e9f80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9f80-123">Authorization</span></span>  | <span data-ttu-id="e9f80-124">string</span><span class="sxs-lookup"><span data-stu-id="e9f80-124">string</span></span>  | <span data-ttu-id="e9f80-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9f80-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9f80-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9f80-127">Request body</span></span>

<span data-ttu-id="e9f80-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9f80-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9f80-129">响应</span><span class="sxs-lookup"><span data-stu-id="e9f80-129">Response</span></span>

<span data-ttu-id="e9f80-130">如果成功，此方法返回 `201 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e9f80-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="e9f80-131">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e9f80-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9f80-132">示例</span><span class="sxs-lookup"><span data-stu-id="e9f80-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e9f80-133">请求</span><span class="sxs-lookup"><span data-stu-id="e9f80-133">Request</span></span>
<span data-ttu-id="e9f80-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e9f80-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="e9f80-135">响应</span><span class="sxs-lookup"><span data-stu-id="e9f80-135">Response</span></span>
<span data-ttu-id="e9f80-136">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e9f80-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
