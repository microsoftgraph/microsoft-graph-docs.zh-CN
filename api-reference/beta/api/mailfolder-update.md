---
title: 更新 mailFolder
description: 更新 mailFolder 对象的属性。
author: angelgolfer-ms
ms.openlocfilehash: d8ae834bd5930d90217a173bea4b5f85f28c0618
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334823"
---
# <a name="update-mailfolder"></a><span data-ttu-id="bf0bc-103">更新 mailFolder</span><span class="sxs-lookup"><span data-stu-id="bf0bc-103">Update mailFolder</span></span>

> <span data-ttu-id="bf0bc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf0bc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf0bc-106">更新[mailFolder](../resources/mailfolder.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-106">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf0bc-107">权限</span><span class="sxs-lookup"><span data-stu-id="bf0bc-107">Permissions</span></span>
<span data-ttu-id="bf0bc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0bc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf0bc-110">Permission type</span></span>      | <span data-ttu-id="bf0bc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf0bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf0bc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf0bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf0bc-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf0bc-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bf0bc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf0bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf0bc-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf0bc-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bf0bc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf0bc-116">Application</span></span> | <span data-ttu-id="bf0bc-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf0bc-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf0bc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf0bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf0bc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf0bc-119">Request headers</span></span>
| <span data-ttu-id="bf0bc-120">标头</span><span class="sxs-lookup"><span data-stu-id="bf0bc-120">Header</span></span>       | <span data-ttu-id="bf0bc-121">值</span><span class="sxs-lookup"><span data-stu-id="bf0bc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf0bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf0bc-122">Authorization</span></span>  | <span data-ttu-id="bf0bc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf0bc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf0bc-125">Content-Type</span></span>  | <span data-ttu-id="bf0bc-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf0bc-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf0bc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf0bc-128">Request body</span></span>
<span data-ttu-id="bf0bc-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bf0bc-132">属性</span><span class="sxs-lookup"><span data-stu-id="bf0bc-132">Property</span></span>     | <span data-ttu-id="bf0bc-133">类型</span><span class="sxs-lookup"><span data-stu-id="bf0bc-133">Type</span></span>   |<span data-ttu-id="bf0bc-134">说明</span><span class="sxs-lookup"><span data-stu-id="bf0bc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf0bc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bf0bc-135">displayName</span></span>|<span data-ttu-id="bf0bc-136">String</span><span class="sxs-lookup"><span data-stu-id="bf0bc-136">String</span></span>|<span data-ttu-id="bf0bc-137">mailFolder 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-137">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="bf0bc-138">响应</span><span class="sxs-lookup"><span data-stu-id="bf0bc-138">Response</span></span>
<span data-ttu-id="bf0bc-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-139">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf0bc-140">示例</span><span class="sxs-lookup"><span data-stu-id="bf0bc-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bf0bc-141">请求</span><span class="sxs-lookup"><span data-stu-id="bf0bc-141">Request</span></span>
<span data-ttu-id="bf0bc-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="bf0bc-143">响应</span><span class="sxs-lookup"><span data-stu-id="bf0bc-143">Response</span></span>
<span data-ttu-id="bf0bc-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-144">The following is an example of the response.</span></span>
><span data-ttu-id="bf0bc-145">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bf0bc-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bf0bc-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
