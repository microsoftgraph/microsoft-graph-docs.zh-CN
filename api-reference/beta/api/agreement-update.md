---
title: 更新协议
description: 更新协议对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: a134e26f6e2b8d2994d960759d389525a80673e4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471563"
---
# <a name="update-agreement"></a><span data-ttu-id="bc035-103">更新协议</span><span class="sxs-lookup"><span data-stu-id="bc035-103">Update agreement</span></span>

<span data-ttu-id="bc035-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc035-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc035-105">更新协议 [对象](../resources/agreement.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="bc035-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc035-106">权限</span><span class="sxs-lookup"><span data-stu-id="bc035-106">Permissions</span></span>
<span data-ttu-id="bc035-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc035-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc035-109">Permission type</span></span>                        | <span data-ttu-id="bc035-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc035-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc035-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc035-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc035-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc035-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="bc035-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc035-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc035-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc035-114">Not supported.</span></span> |
|<span data-ttu-id="bc035-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc035-115">Application</span></span>                            | <span data-ttu-id="bc035-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc035-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc035-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc035-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bc035-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc035-118">Request headers</span></span>
| <span data-ttu-id="bc035-119">名称</span><span class="sxs-lookup"><span data-stu-id="bc035-119">Name</span></span>         | <span data-ttu-id="bc035-120">类型</span><span class="sxs-lookup"><span data-stu-id="bc035-120">Type</span></span>        | <span data-ttu-id="bc035-121">说明</span><span class="sxs-lookup"><span data-stu-id="bc035-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bc035-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc035-122">Authorization</span></span> | <span data-ttu-id="bc035-123">string</span><span class="sxs-lookup"><span data-stu-id="bc035-123">string</span></span> | <span data-ttu-id="bc035-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc035-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc035-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc035-126">Request body</span></span>
<span data-ttu-id="bc035-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bc035-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bc035-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bc035-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bc035-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bc035-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc035-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc035-130">Property</span></span>     | <span data-ttu-id="bc035-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc035-131">Type</span></span>        | <span data-ttu-id="bc035-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc035-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc035-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bc035-133">displayName</span></span>|<span data-ttu-id="bc035-134">String</span><span class="sxs-lookup"><span data-stu-id="bc035-134">String</span></span>|<span data-ttu-id="bc035-135">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc035-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="bc035-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="bc035-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="bc035-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc035-137">Boolean</span></span>|<span data-ttu-id="bc035-138">用户在接受之前是否必须展开和查看协议。</span><span class="sxs-lookup"><span data-stu-id="bc035-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="bc035-139">响应</span><span class="sxs-lookup"><span data-stu-id="bc035-139">Response</span></span>
<span data-ttu-id="bc035-140">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新[](../resources/agreement.md)的协议对象。</span><span class="sxs-lookup"><span data-stu-id="bc035-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc035-141">示例</span><span class="sxs-lookup"><span data-stu-id="bc035-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc035-142">请求</span><span class="sxs-lookup"><span data-stu-id="bc035-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```

##### <a name="response"></a><span data-ttu-id="bc035-143">响应</span><span class="sxs-lookup"><span data-stu-id="bc035-143">Response</span></span>
><span data-ttu-id="bc035-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bc035-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->


