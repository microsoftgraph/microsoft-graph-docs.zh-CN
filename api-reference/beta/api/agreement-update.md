---
title: 更新协议
description: 更新协议对象的属性。
localization_priority: Normal
ms.openlocfilehash: fc6e4718a026f78a6e892dc13095492099b654cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520065"
---
# <a name="update-agreement"></a><span data-ttu-id="37f3c-103">更新协议</span><span class="sxs-lookup"><span data-stu-id="37f3c-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f3c-104">更新[协议](../resources/agreement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="37f3c-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37f3c-105">权限</span><span class="sxs-lookup"><span data-stu-id="37f3c-105">Permissions</span></span>
<span data-ttu-id="37f3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f3c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="37f3c-108">Permission type</span></span>                        | <span data-ttu-id="37f3c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37f3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="37f3c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37f3c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="37f3c-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f3c-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="37f3c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37f3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37f3c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f3c-113">Not supported.</span></span> |
|<span data-ttu-id="37f3c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="37f3c-114">Application</span></span>                            | <span data-ttu-id="37f3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37f3c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37f3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="37f3c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="37f3c-117">Request headers</span></span>
| <span data-ttu-id="37f3c-118">名称</span><span class="sxs-lookup"><span data-stu-id="37f3c-118">Name</span></span>         | <span data-ttu-id="37f3c-119">类型</span><span class="sxs-lookup"><span data-stu-id="37f3c-119">Type</span></span>        | <span data-ttu-id="37f3c-120">说明</span><span class="sxs-lookup"><span data-stu-id="37f3c-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="37f3c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f3c-121">Authorization</span></span> | <span data-ttu-id="37f3c-122">字符串</span><span class="sxs-lookup"><span data-stu-id="37f3c-122">string</span></span> | <span data-ttu-id="37f3c-123">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="37f3c-123">Bearer \{token\}.</span></span> <span data-ttu-id="37f3c-124">必需。</span><span class="sxs-lookup"><span data-stu-id="37f3c-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37f3c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="37f3c-125">Request body</span></span>
<span data-ttu-id="37f3c-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="37f3c-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="37f3c-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="37f3c-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="37f3c-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="37f3c-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="37f3c-129">属性</span><span class="sxs-lookup"><span data-stu-id="37f3c-129">Property</span></span>     | <span data-ttu-id="37f3c-130">类型</span><span class="sxs-lookup"><span data-stu-id="37f3c-130">Type</span></span>        | <span data-ttu-id="37f3c-131">说明</span><span class="sxs-lookup"><span data-stu-id="37f3c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37f3c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="37f3c-132">displayName</span></span>|<span data-ttu-id="37f3c-133">String</span><span class="sxs-lookup"><span data-stu-id="37f3c-133">String</span></span>|<span data-ttu-id="37f3c-134">协议中的显示名称。</span><span class="sxs-lookup"><span data-stu-id="37f3c-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="37f3c-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="37f3c-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="37f3c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f3c-136">Boolean</span></span>|<span data-ttu-id="37f3c-137">用户是否能够展开和查看接受之前协议。</span><span class="sxs-lookup"><span data-stu-id="37f3c-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="37f3c-138">响应</span><span class="sxs-lookup"><span data-stu-id="37f3c-138">Response</span></span>
<span data-ttu-id="37f3c-139">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="37f3c-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37f3c-140">示例</span><span class="sxs-lookup"><span data-stu-id="37f3c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37f3c-141">请求</span><span class="sxs-lookup"><span data-stu-id="37f3c-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="37f3c-142">响应</span><span class="sxs-lookup"><span data-stu-id="37f3c-142">Response</span></span>
><span data-ttu-id="37f3c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="37f3c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
