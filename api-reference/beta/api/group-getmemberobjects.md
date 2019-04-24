---
title: 'group: getMemberObjects'
description: 返回组所属的所有组和管理单元。 检查是可传递的。 注意：组不能是目录角色的成员，因此不会返回任何目录角色。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4b71a683d3c311acc36ca0ab669c5d6d44180f31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502394"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="63722-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="63722-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63722-106">返回组所属的所有组和管理单元。</span><span class="sxs-lookup"><span data-stu-id="63722-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="63722-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="63722-107">The check is transitive.</span></span> <span data-ttu-id="63722-108">注意：组不能是目录角色的成员，因此不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="63722-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="63722-109">权限</span><span class="sxs-lookup"><span data-stu-id="63722-109">Permissions</span></span>
<span data-ttu-id="63722-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63722-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63722-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="63722-112">Permission type</span></span>      | <span data-ttu-id="63722-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63722-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63722-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63722-114">Delegated (work or school account)</span></span> | <span data-ttu-id="63722-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63722-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63722-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63722-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63722-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="63722-117">Not supported.</span></span>    |
|<span data-ttu-id="63722-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="63722-118">Application</span></span> | <span data-ttu-id="63722-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63722-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63722-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63722-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="63722-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="63722-121">Request headers</span></span>
| <span data-ttu-id="63722-122">名称</span><span class="sxs-lookup"><span data-stu-id="63722-122">Name</span></span>       | <span data-ttu-id="63722-123">类型</span><span class="sxs-lookup"><span data-stu-id="63722-123">Type</span></span> | <span data-ttu-id="63722-124">说明</span><span class="sxs-lookup"><span data-stu-id="63722-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="63722-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63722-125">Authorization</span></span>  | <span data-ttu-id="63722-126">string</span><span class="sxs-lookup"><span data-stu-id="63722-126">string</span></span>  | <span data-ttu-id="63722-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63722-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63722-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="63722-129">Request body</span></span>
<span data-ttu-id="63722-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="63722-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63722-131">参数</span><span class="sxs-lookup"><span data-stu-id="63722-131">Parameter</span></span>    | <span data-ttu-id="63722-132">类型</span><span class="sxs-lookup"><span data-stu-id="63722-132">Type</span></span>   |<span data-ttu-id="63722-133">说明</span><span class="sxs-lookup"><span data-stu-id="63722-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63722-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="63722-134">securityEnabledOnly</span></span>|<span data-ttu-id="63722-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="63722-135">Boolean</span></span>|<span data-ttu-id="63722-p105">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="63722-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="63722-138">响应</span><span class="sxs-lookup"><span data-stu-id="63722-138">Response</span></span>
<span data-ttu-id="63722-139">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="63722-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="63722-140">示例</span><span class="sxs-lookup"><span data-stu-id="63722-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="63722-141">请求</span><span class="sxs-lookup"><span data-stu-id="63722-141">Request</span></span>
<span data-ttu-id="63722-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63722-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="63722-143">响应</span><span class="sxs-lookup"><span data-stu-id="63722-143">Response</span></span>
<span data-ttu-id="63722-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63722-144">The following is an example of the response.</span></span>
><span data-ttu-id="63722-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63722-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
