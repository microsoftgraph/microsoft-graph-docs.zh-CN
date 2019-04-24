---
title: 创建 sectionGroup
description: 在指定分区组中新建分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a05e61934c8043c0c6a94c6e0785c0e93e4a3e19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520926"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="c4950-103">创建 sectionGroup</span><span class="sxs-lookup"><span data-stu-id="c4950-103">Create sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4950-104">在指定分区组中新建[分区组](../resources/sectiongroup.md)。</span><span class="sxs-lookup"><span data-stu-id="c4950-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4950-105">权限</span><span class="sxs-lookup"><span data-stu-id="c4950-105">Permissions</span></span>
<span data-ttu-id="c4950-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4950-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4950-108">Permission type</span></span>      | <span data-ttu-id="c4950-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4950-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4950-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4950-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4950-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4950-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4950-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4950-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4950-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4950-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c4950-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4950-114">Application</span></span> | <span data-ttu-id="c4950-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4950-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4950-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4950-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="c4950-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4950-117">Request headers</span></span>
| <span data-ttu-id="c4950-118">名称</span><span class="sxs-lookup"><span data-stu-id="c4950-118">Name</span></span>       | <span data-ttu-id="c4950-119">类型</span><span class="sxs-lookup"><span data-stu-id="c4950-119">Type</span></span> | <span data-ttu-id="c4950-120">说明</span><span class="sxs-lookup"><span data-stu-id="c4950-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4950-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4950-121">Authorization</span></span>  | <span data-ttu-id="c4950-122">string</span><span class="sxs-lookup"><span data-stu-id="c4950-122">string</span></span>  | <span data-ttu-id="c4950-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4950-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4950-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4950-125">Content-Type</span></span> | <span data-ttu-id="c4950-126">string</span><span class="sxs-lookup"><span data-stu-id="c4950-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c4950-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4950-127">Request body</span></span>
<span data-ttu-id="c4950-128">在请求正文中，提供分区组名称。</span><span class="sxs-lookup"><span data-stu-id="c4950-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="c4950-p103">在同一个层次结构级别中，分区组名称必须是唯一的。该名称不能超过 50 个字符，也不能包含以下字符：?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="c4950-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="c4950-131">响应</span><span class="sxs-lookup"><span data-stu-id="c4950-131">Response</span></span>

<span data-ttu-id="c4950-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4950-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4950-133">示例</span><span class="sxs-lookup"><span data-stu-id="c4950-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4950-134">请求</span><span class="sxs-lookup"><span data-stu-id="c4950-134">Request</span></span>
<span data-ttu-id="c4950-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4950-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c4950-136">响应</span><span class="sxs-lookup"><span data-stu-id="c4950-136">Response</span></span>
<span data-ttu-id="c4950-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4950-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-post-sectiongroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
