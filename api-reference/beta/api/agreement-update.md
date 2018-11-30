---
title: 更新协议
description: 更新协议对象的属性。
ms.openlocfilehash: b9405a8c469876a349b5c1b0c00e6f6a5f225e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042409"
---
# <a name="update-agreement"></a><span data-ttu-id="49f64-103">更新协议</span><span class="sxs-lookup"><span data-stu-id="49f64-103">Update agreement</span></span>

> <span data-ttu-id="49f64-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49f64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49f64-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49f64-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49f64-106">更新[协议](../resources/agreement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="49f64-106">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49f64-107">权限</span><span class="sxs-lookup"><span data-stu-id="49f64-107">Permissions</span></span>
<span data-ttu-id="49f64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49f64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="49f64-110">Permission type</span></span>                        | <span data-ttu-id="49f64-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49f64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="49f64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49f64-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="49f64-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f64-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="49f64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49f64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49f64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="49f64-115">Not supported.</span></span> |
|<span data-ttu-id="49f64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="49f64-116">Application</span></span>                            | <span data-ttu-id="49f64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="49f64-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49f64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49f64-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="49f64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="49f64-119">Request headers</span></span>
| <span data-ttu-id="49f64-120">名称</span><span class="sxs-lookup"><span data-stu-id="49f64-120">Name</span></span>         | <span data-ttu-id="49f64-121">类型</span><span class="sxs-lookup"><span data-stu-id="49f64-121">Type</span></span>        | <span data-ttu-id="49f64-122">说明</span><span class="sxs-lookup"><span data-stu-id="49f64-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="49f64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49f64-123">Authorization</span></span> | <span data-ttu-id="49f64-124">string</span><span class="sxs-lookup"><span data-stu-id="49f64-124">string</span></span> | <span data-ttu-id="49f64-125">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="49f64-125">Bearer \{token\}.</span></span> <span data-ttu-id="49f64-126">必需。</span><span class="sxs-lookup"><span data-stu-id="49f64-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49f64-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="49f64-127">Request body</span></span>
<span data-ttu-id="49f64-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="49f64-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="49f64-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="49f64-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="49f64-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="49f64-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="49f64-131">属性</span><span class="sxs-lookup"><span data-stu-id="49f64-131">Property</span></span>     | <span data-ttu-id="49f64-132">类型</span><span class="sxs-lookup"><span data-stu-id="49f64-132">Type</span></span>        | <span data-ttu-id="49f64-133">说明</span><span class="sxs-lookup"><span data-stu-id="49f64-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="49f64-134">displayName</span><span class="sxs-lookup"><span data-stu-id="49f64-134">displayName</span></span>|<span data-ttu-id="49f64-135">字符串</span><span class="sxs-lookup"><span data-stu-id="49f64-135">String</span></span>|<span data-ttu-id="49f64-136">协议中的显示名称。</span><span class="sxs-lookup"><span data-stu-id="49f64-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="49f64-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="49f64-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="49f64-138">布尔</span><span class="sxs-lookup"><span data-stu-id="49f64-138">Boolean</span></span>|<span data-ttu-id="49f64-139">用户是否能够展开和查看接受之前协议。</span><span class="sxs-lookup"><span data-stu-id="49f64-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="49f64-140">响应</span><span class="sxs-lookup"><span data-stu-id="49f64-140">Response</span></span>
<span data-ttu-id="49f64-141">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49f64-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49f64-142">示例</span><span class="sxs-lookup"><span data-stu-id="49f64-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49f64-143">请求</span><span class="sxs-lookup"><span data-stu-id="49f64-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="49f64-144">响应</span><span class="sxs-lookup"><span data-stu-id="49f64-144">Response</span></span>
><span data-ttu-id="49f64-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49f64-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
