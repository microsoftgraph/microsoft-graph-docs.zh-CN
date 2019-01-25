---
title: 更新 oAuth2PermissionGrant
description: 更新 oAuth2PermissionGrant 对象的属性。
localization_priority: Normal
ms.openlocfilehash: fb990c56b4d7ae62ac35935a91d69688b96bff28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522138"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="d32a3-103">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d32a3-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d32a3-104">更新 oAuth2PermissionGrant 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d32a3-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d32a3-105">权限</span><span class="sxs-lookup"><span data-stu-id="d32a3-105">Permissions</span></span>

<span data-ttu-id="d32a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d32a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d32a3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d32a3-108">Permission type</span></span>      | <span data-ttu-id="d32a3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d32a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d32a3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d32a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d32a3-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d32a3-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d32a3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d32a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d32a3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d32a3-113">Not supported.</span></span>    |
|<span data-ttu-id="d32a3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d32a3-114">Application</span></span> | <span data-ttu-id="d32a3-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d32a3-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d32a3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d32a3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d32a3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d32a3-117">Request headers</span></span>
| <span data-ttu-id="d32a3-118">名称</span><span class="sxs-lookup"><span data-stu-id="d32a3-118">Name</span></span>       | <span data-ttu-id="d32a3-119">类型</span><span class="sxs-lookup"><span data-stu-id="d32a3-119">Type</span></span> | <span data-ttu-id="d32a3-120">说明</span><span class="sxs-lookup"><span data-stu-id="d32a3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d32a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d32a3-121">Authorization</span></span>  | <span data-ttu-id="d32a3-122">string</span><span class="sxs-lookup"><span data-stu-id="d32a3-122">string</span></span>  | <span data-ttu-id="d32a3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d32a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d32a3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d32a3-125">Request body</span></span>
<span data-ttu-id="d32a3-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d32a3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d32a3-129">属性</span><span class="sxs-lookup"><span data-stu-id="d32a3-129">Property</span></span>     | <span data-ttu-id="d32a3-130">类型</span><span class="sxs-lookup"><span data-stu-id="d32a3-130">Type</span></span>   |<span data-ttu-id="d32a3-131">说明</span><span class="sxs-lookup"><span data-stu-id="d32a3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d32a3-132">scope</span><span class="sxs-lookup"><span data-stu-id="d32a3-132">scope</span></span>|<span data-ttu-id="d32a3-133">String</span><span class="sxs-lookup"><span data-stu-id="d32a3-133">String</span></span>| <span data-ttu-id="d32a3-134">OAuth 2.0 访问令牌中指定资源应用程序应产生预期范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="d32a3-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="d32a3-135">响应</span><span class="sxs-lookup"><span data-stu-id="d32a3-135">Response</span></span>

<span data-ttu-id="d32a3-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d32a3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d32a3-138">示例</span><span class="sxs-lookup"><span data-stu-id="d32a3-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d32a3-139">请求</span><span class="sxs-lookup"><span data-stu-id="d32a3-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
##### <a name="response"></a><span data-ttu-id="d32a3-140">响应</span><span class="sxs-lookup"><span data-stu-id="d32a3-140">Response</span></span>

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
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
