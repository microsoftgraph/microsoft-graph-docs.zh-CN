---
title: 创建分区
description: 在指定的笔记本中新建分区。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: c6c091d399ae2b9fc69d249a3e2a34f3051c1611
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892461"
---
# <a name="create-section"></a><span data-ttu-id="72bec-103">创建分区</span><span class="sxs-lookup"><span data-stu-id="72bec-103">Create section</span></span>

> <span data-ttu-id="72bec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="72bec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72bec-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="72bec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72bec-106">在指定的笔记本中新建[分区](../resources/section.md)。</span><span class="sxs-lookup"><span data-stu-id="72bec-106">Create a new [section](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="72bec-107">权限</span><span class="sxs-lookup"><span data-stu-id="72bec-107">Permissions</span></span>
<span data-ttu-id="72bec-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72bec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72bec-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72bec-110">Permission type</span></span>      | <span data-ttu-id="72bec-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72bec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72bec-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72bec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72bec-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bec-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="72bec-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72bec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72bec-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72bec-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="72bec-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72bec-116">Application</span></span> | <span data-ttu-id="72bec-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bec-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72bec-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72bec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="72bec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72bec-119">Request headers</span></span>
| <span data-ttu-id="72bec-120">名称</span><span class="sxs-lookup"><span data-stu-id="72bec-120">Name</span></span>       | <span data-ttu-id="72bec-121">类型</span><span class="sxs-lookup"><span data-stu-id="72bec-121">Type</span></span> | <span data-ttu-id="72bec-122">说明</span><span class="sxs-lookup"><span data-stu-id="72bec-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="72bec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72bec-123">Authorization</span></span>  | <span data-ttu-id="72bec-124">string</span><span class="sxs-lookup"><span data-stu-id="72bec-124">string</span></span>  | <span data-ttu-id="72bec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72bec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72bec-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72bec-127">Content-Type</span></span> | <span data-ttu-id="72bec-128">string</span><span class="sxs-lookup"><span data-stu-id="72bec-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="72bec-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="72bec-129">Request body</span></span>
<span data-ttu-id="72bec-130">在请求正文中，提供分区名称。</span><span class="sxs-lookup"><span data-stu-id="72bec-130">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="72bec-p104">在同一个层次结构级别中，分区名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="72bec-p104">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="72bec-133">响应</span><span class="sxs-lookup"><span data-stu-id="72bec-133">Response</span></span>

<span data-ttu-id="72bec-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [section](../resources/section.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72bec-134">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72bec-135">示例</span><span class="sxs-lookup"><span data-stu-id="72bec-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72bec-136">请求</span><span class="sxs-lookup"><span data-stu-id="72bec-136">Request</span></span>
<span data-ttu-id="72bec-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72bec-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="72bec-138">响应</span><span class="sxs-lookup"><span data-stu-id="72bec-138">Response</span></span>
<span data-ttu-id="72bec-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72bec-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
