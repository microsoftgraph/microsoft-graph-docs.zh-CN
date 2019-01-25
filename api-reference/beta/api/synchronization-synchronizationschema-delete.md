---
title: 删除 synchronizationSchema
description: 删除自定义的架构，并将架构重置为默认配置。 如果模板的上下文中删除架构，则它将重置架构为一个相关联的模板的默认`factoryTag`。
localization_priority: Normal
ms.openlocfilehash: cb4c6295fe962ea9570da19b9b6ee8190b2024f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526989"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="dc5b4-104">删除 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="dc5b4-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc5b4-105">删除自定义的架构，并将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="dc5b4-106">如果模板的上下文中删除架构，则它将重置架构为一个相关联的模板的默认`factoryTag`。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc5b4-107">权限</span><span class="sxs-lookup"><span data-stu-id="dc5b4-107">Permissions</span></span>
<span data-ttu-id="dc5b4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc5b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc5b4-110">Permission type</span></span>                        | <span data-ttu-id="dc5b4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc5b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc5b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc5b4-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="dc5b4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc5b4-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="dc5b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc5b4-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="dc5b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-115">Not supported.</span></span>|
|<span data-ttu-id="dc5b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc5b4-116">Application</span></span>                            |<span data-ttu-id="dc5b4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="dc5b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc5b4-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="dc5b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc5b4-119">Request headers</span></span>

| <span data-ttu-id="dc5b4-120">名称</span><span class="sxs-lookup"><span data-stu-id="dc5b4-120">Name</span></span>           | <span data-ttu-id="dc5b4-121">类型</span><span class="sxs-lookup"><span data-stu-id="dc5b4-121">Type</span></span>    | <span data-ttu-id="dc5b4-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc5b4-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="dc5b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc5b4-123">Authorization</span></span>  | <span data-ttu-id="dc5b4-124">string</span><span class="sxs-lookup"><span data-stu-id="dc5b4-124">string</span></span>  | <span data-ttu-id="dc5b4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc5b4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc5b4-127">Request body</span></span>

<span data-ttu-id="dc5b4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc5b4-129">响应</span><span class="sxs-lookup"><span data-stu-id="dc5b4-129">Response</span></span>

<span data-ttu-id="dc5b4-130">如果成功，此方法返回 `201 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="dc5b4-131">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc5b4-132">示例</span><span class="sxs-lookup"><span data-stu-id="dc5b4-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc5b4-133">请求</span><span class="sxs-lookup"><span data-stu-id="dc5b4-133">Request</span></span>
<span data-ttu-id="dc5b4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="dc5b4-135">响应</span><span class="sxs-lookup"><span data-stu-id="dc5b4-135">Response</span></span>
<span data-ttu-id="dc5b4-136">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="dc5b4-136">The following is an example of a response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
