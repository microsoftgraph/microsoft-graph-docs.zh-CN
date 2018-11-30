---
title: 创建 sectionGroup
description: 在指定分区组中新建分区组。
ms.openlocfilehash: 62e88f65755006fb6cbb4755cd63ef02fbc19556
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044647"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="2c3a2-103">创建 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="2c3a2-103">Create sectionGroup</span></span>

> <span data-ttu-id="2c3a2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c3a2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c3a2-106">在指定分区组中新建[分区组](../resources/sectiongroup.md)。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-106">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c3a2-107">权限</span><span class="sxs-lookup"><span data-stu-id="2c3a2-107">Permissions</span></span>
<span data-ttu-id="2c3a2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c3a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c3a2-110">Permission type</span></span>      | <span data-ttu-id="2c3a2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c3a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c3a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c3a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c3a2-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c3a2-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c3a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c3a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c3a2-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c3a2-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2c3a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c3a2-116">Application</span></span> | <span data-ttu-id="2c3a2-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c3a2-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c3a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c3a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="2c3a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c3a2-119">Request headers</span></span>
| <span data-ttu-id="2c3a2-120">名称</span><span class="sxs-lookup"><span data-stu-id="2c3a2-120">Name</span></span>       | <span data-ttu-id="2c3a2-121">类型</span><span class="sxs-lookup"><span data-stu-id="2c3a2-121">Type</span></span> | <span data-ttu-id="2c3a2-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c3a2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c3a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c3a2-123">Authorization</span></span>  | <span data-ttu-id="2c3a2-124">string</span><span class="sxs-lookup"><span data-stu-id="2c3a2-124">string</span></span>  | <span data-ttu-id="2c3a2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c3a2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c3a2-127">Content-Type</span></span> | <span data-ttu-id="2c3a2-128">string</span><span class="sxs-lookup"><span data-stu-id="2c3a2-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2c3a2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c3a2-129">Request body</span></span>
<span data-ttu-id="2c3a2-130">在请求正文中，提供分区组名称。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="2c3a2-p104">在同一个层次结构级别中，分区组名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="2c3a2-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="2c3a2-133">响应</span><span class="sxs-lookup"><span data-stu-id="2c3a2-133">Response</span></span>

<span data-ttu-id="2c3a2-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-134">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c3a2-135">示例</span><span class="sxs-lookup"><span data-stu-id="2c3a2-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c3a2-136">请求</span><span class="sxs-lookup"><span data-stu-id="2c3a2-136">Request</span></span>
<span data-ttu-id="2c3a2-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="2c3a2-138">响应</span><span class="sxs-lookup"><span data-stu-id="2c3a2-138">Response</span></span>
<span data-ttu-id="2c3a2-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c3a2-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
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
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->