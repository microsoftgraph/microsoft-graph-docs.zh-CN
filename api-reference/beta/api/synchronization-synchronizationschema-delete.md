---
title: 删除 synchronizationSchema
description: 删除自定义架构并将架构重置为默认配置。 如果在模板的上下文中删除了架构，它会将架构重置为与模板关联的默认架构`factoryTag`。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de8e8eaf2d8a5473a530c8497aca7e40739ed19c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443355"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="a7fb4-104">删除 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="a7fb4-104">Delete synchronizationSchema</span></span>

<span data-ttu-id="a7fb4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7fb4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7fb4-106">删除自定义架构并将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-106">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="a7fb4-107">如果在模板的上下文中删除了架构，它会将架构重置为与模板关联的默认架构`factoryTag`。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-107">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7fb4-108">权限</span><span class="sxs-lookup"><span data-stu-id="a7fb4-108">Permissions</span></span>
<span data-ttu-id="a7fb4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7fb4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7fb4-111">Permission type</span></span>                        | <span data-ttu-id="a7fb4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7fb4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7fb4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7fb4-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="a7fb4-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7fb4-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a7fb4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7fb4-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a7fb4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-116">Not supported.</span></span>|
|<span data-ttu-id="a7fb4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7fb4-117">Application</span></span>                            |<span data-ttu-id="a7fb4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="a7fb4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7fb4-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="a7fb4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7fb4-120">Request headers</span></span>

| <span data-ttu-id="a7fb4-121">名称</span><span class="sxs-lookup"><span data-stu-id="a7fb4-121">Name</span></span>           | <span data-ttu-id="a7fb4-122">类型</span><span class="sxs-lookup"><span data-stu-id="a7fb4-122">Type</span></span>    | <span data-ttu-id="a7fb4-123">说明</span><span class="sxs-lookup"><span data-stu-id="a7fb4-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a7fb4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7fb4-124">Authorization</span></span>  | <span data-ttu-id="a7fb4-125">string</span><span class="sxs-lookup"><span data-stu-id="a7fb4-125">string</span></span>  | <span data-ttu-id="a7fb4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7fb4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7fb4-128">Request body</span></span>

<span data-ttu-id="a7fb4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7fb4-130">响应</span><span class="sxs-lookup"><span data-stu-id="a7fb4-130">Response</span></span>

<span data-ttu-id="a7fb4-131">如果成功，此方法返回 `201 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-131">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="a7fb4-132">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-132">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7fb4-133">示例</span><span class="sxs-lookup"><span data-stu-id="a7fb4-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a7fb4-134">请求</span><span class="sxs-lookup"><span data-stu-id="a7fb4-134">Request</span></span>
<span data-ttu-id="a7fb4-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-135">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="a7fb4-136">响应</span><span class="sxs-lookup"><span data-stu-id="a7fb4-136">Response</span></span>
<span data-ttu-id="a7fb4-137">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a7fb4-137">The following is an example of a response.</span></span>
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
