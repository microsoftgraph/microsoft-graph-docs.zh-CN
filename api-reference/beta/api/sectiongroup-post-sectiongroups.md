---
title: 创建 sectionGroup
description: 在指定分区组中新建分区组。
localization_priority: Normal
ms.openlocfilehash: 5af01bd2a526d692b568fe121db7933a2887a006
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812955"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="dbbee-103">创建 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="dbbee-103">Create sectionGroup</span></span>

> <span data-ttu-id="dbbee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dbbee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbbee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dbbee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbbee-106">在指定分区组中新建[分区组](../resources/sectiongroup.md)。</span><span class="sxs-lookup"><span data-stu-id="dbbee-106">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbbee-107">权限</span><span class="sxs-lookup"><span data-stu-id="dbbee-107">Permissions</span></span>
<span data-ttu-id="dbbee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbbee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbbee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbbee-110">Permission type</span></span>      | <span data-ttu-id="dbbee-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbbee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbbee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbbee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dbbee-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbbee-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbbee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbbee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbbee-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbbee-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dbbee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbbee-116">Application</span></span> | <span data-ttu-id="dbbee-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbbee-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbbee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbbee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="dbbee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbbee-119">Request headers</span></span>
| <span data-ttu-id="dbbee-120">名称</span><span class="sxs-lookup"><span data-stu-id="dbbee-120">Name</span></span>       | <span data-ttu-id="dbbee-121">类型</span><span class="sxs-lookup"><span data-stu-id="dbbee-121">Type</span></span> | <span data-ttu-id="dbbee-122">说明</span><span class="sxs-lookup"><span data-stu-id="dbbee-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbbee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbbee-123">Authorization</span></span>  | <span data-ttu-id="dbbee-124">string</span><span class="sxs-lookup"><span data-stu-id="dbbee-124">string</span></span>  | <span data-ttu-id="dbbee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dbbee-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbbee-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbbee-127">Content-Type</span></span> | <span data-ttu-id="dbbee-128">string</span><span class="sxs-lookup"><span data-stu-id="dbbee-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dbbee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbbee-129">Request body</span></span>
<span data-ttu-id="dbbee-130">在请求正文中，提供分区组名称。</span><span class="sxs-lookup"><span data-stu-id="dbbee-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="dbbee-p104">在同一个层次结构级别中，分区组名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="dbbee-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="dbbee-133">响应</span><span class="sxs-lookup"><span data-stu-id="dbbee-133">Response</span></span>

<span data-ttu-id="dbbee-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbbee-134">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbbee-135">示例</span><span class="sxs-lookup"><span data-stu-id="dbbee-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbbee-136">请求</span><span class="sxs-lookup"><span data-stu-id="dbbee-136">Request</span></span>
<span data-ttu-id="dbbee-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbbee-137">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="dbbee-138">响应</span><span class="sxs-lookup"><span data-stu-id="dbbee-138">Response</span></span>
<span data-ttu-id="dbbee-p105">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbbee-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
