---
title: 删除 schemaExtension
description: 删除架构扩展定义。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 96b7ab5091d7e8a33bd3e94fea4a9ccc85a686fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962798"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="190fe-103">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="190fe-103">Delete schemaExtension</span></span>

> <span data-ttu-id="190fe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="190fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="190fe-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="190fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="190fe-106">删除[架构扩展](../resources/schemaextension.md)定义。</span><span class="sxs-lookup"><span data-stu-id="190fe-106">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="190fe-p102">仅创建架构扩展的应用（所有者应用）可以删除架构扩展定义，并且仅在该扩展处于 **InDevelopment** 状态下时才可以将其删除。删除架构扩展定义不会影响访问基于此定义已添加到资源实例的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="190fe-p102">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="190fe-109">权限</span><span class="sxs-lookup"><span data-stu-id="190fe-109">Permissions</span></span>
<span data-ttu-id="190fe-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="190fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="190fe-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="190fe-112">Permission type</span></span>      | <span data-ttu-id="190fe-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="190fe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="190fe-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="190fe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="190fe-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="190fe-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="190fe-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="190fe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="190fe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="190fe-117">Not supported.</span></span>    |
|<span data-ttu-id="190fe-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="190fe-118">Application</span></span> | <span data-ttu-id="190fe-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="190fe-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="190fe-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="190fe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="190fe-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="190fe-121">Request headers</span></span>
| <span data-ttu-id="190fe-122">名称</span><span class="sxs-lookup"><span data-stu-id="190fe-122">Name</span></span>      |<span data-ttu-id="190fe-123">说明</span><span class="sxs-lookup"><span data-stu-id="190fe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="190fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="190fe-124">Authorization</span></span>  | <span data-ttu-id="190fe-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="190fe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="190fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="190fe-127">Request body</span></span>
<span data-ttu-id="190fe-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="190fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="190fe-129">响应</span><span class="sxs-lookup"><span data-stu-id="190fe-129">Response</span></span>

<span data-ttu-id="190fe-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="190fe-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="190fe-132">示例</span><span class="sxs-lookup"><span data-stu-id="190fe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="190fe-133">请求</span><span class="sxs-lookup"><span data-stu-id="190fe-133">Request</span></span>
<span data-ttu-id="190fe-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="190fe-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="190fe-135">响应</span><span class="sxs-lookup"><span data-stu-id="190fe-135">Response</span></span>
<span data-ttu-id="190fe-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="190fe-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="190fe-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="190fe-137">See also</span></span>

- [<span data-ttu-id="190fe-138">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="190fe-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="190fe-139">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="190fe-139">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
