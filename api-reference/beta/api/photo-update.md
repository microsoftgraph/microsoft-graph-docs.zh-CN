---
title: 更新照片
description: 更新 photo 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 4db957b18ea65c8e65f8b446229b57a6f627fad0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521507"
---
# <a name="update-photo"></a><span data-ttu-id="0c600-103">更新照片</span><span class="sxs-lookup"><span data-stu-id="0c600-103">Update photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c600-104">更新 photo 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0c600-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c600-105">权限</span><span class="sxs-lookup"><span data-stu-id="0c600-105">Permissions</span></span>
<span data-ttu-id="0c600-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c600-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c600-108">Permission type</span></span>      | <span data-ttu-id="0c600-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c600-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c600-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c600-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c600-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c600-111">Not supported.</span></span>    |
|<span data-ttu-id="0c600-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c600-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c600-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c600-113">Not supported.</span></span>    |
|<span data-ttu-id="0c600-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c600-114">Application</span></span> | <span data-ttu-id="0c600-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c600-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c600-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c600-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="0c600-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c600-117">Request headers</span></span>
| <span data-ttu-id="0c600-118">名称</span><span class="sxs-lookup"><span data-stu-id="0c600-118">Name</span></span>       | <span data-ttu-id="0c600-119">类型</span><span class="sxs-lookup"><span data-stu-id="0c600-119">Type</span></span> | <span data-ttu-id="0c600-120">说明</span><span class="sxs-lookup"><span data-stu-id="0c600-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c600-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c600-121">Authorization</span></span>  | <span data-ttu-id="0c600-122">string</span><span class="sxs-lookup"><span data-stu-id="0c600-122">string</span></span>  | <span data-ttu-id="0c600-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c600-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c600-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c600-125">Request body</span></span>
<span data-ttu-id="0c600-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0c600-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c600-129">属性</span><span class="sxs-lookup"><span data-stu-id="0c600-129">Property</span></span>     | <span data-ttu-id="0c600-130">类型</span><span class="sxs-lookup"><span data-stu-id="0c600-130">Type</span></span>   |<span data-ttu-id="0c600-131">说明</span><span class="sxs-lookup"><span data-stu-id="0c600-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="0c600-132">响应</span><span class="sxs-lookup"><span data-stu-id="0c600-132">Response</span></span>

<span data-ttu-id="0c600-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c600-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c600-134">示例</span><span class="sxs-lookup"><span data-stu-id="0c600-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c600-135">请求</span><span class="sxs-lookup"><span data-stu-id="0c600-135">Request</span></span>
<span data-ttu-id="0c600-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c600-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="0c600-137">响应</span><span class="sxs-lookup"><span data-stu-id="0c600-137">Response</span></span>
<span data-ttu-id="0c600-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0c600-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/photo-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
