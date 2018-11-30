---
title: 更新目录设置
description: 更新特定目录设置对象的属性。
ms.openlocfilehash: 71568cdbd2a58bddbd40fffe20616616ff7398eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046107"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="79df9-103">更新目录设置</span><span class="sxs-lookup"><span data-stu-id="79df9-103">Update a directory setting</span></span>

> <span data-ttu-id="79df9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="79df9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79df9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="79df9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79df9-106">更新特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="79df9-106">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="79df9-107">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="79df9-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="79df9-108">此 API 的 /v1.0 版本已被重命名为*更新 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="79df9-108">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="79df9-109">权限</span><span class="sxs-lookup"><span data-stu-id="79df9-109">Permissions</span></span>
<span data-ttu-id="79df9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79df9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79df9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="79df9-112">Permission type</span></span>      | <span data-ttu-id="79df9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79df9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79df9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79df9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="79df9-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79df9-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79df9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79df9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79df9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79df9-117">Not supported.</span></span>    |
|<span data-ttu-id="79df9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="79df9-118">Application</span></span> | <span data-ttu-id="79df9-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79df9-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79df9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79df9-120">HTTP request</span></span>
<span data-ttu-id="79df9-121"><!-- { "blockType": "ignored" } -->更新租户范围内或组的特定设置。</span><span class="sxs-lookup"><span data-stu-id="79df9-121"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="79df9-122">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="79df9-122">Optional request headers</span></span>
| <span data-ttu-id="79df9-123">名称</span><span class="sxs-lookup"><span data-stu-id="79df9-123">Name</span></span>       | <span data-ttu-id="79df9-124">说明</span><span class="sxs-lookup"><span data-stu-id="79df9-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="79df9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="79df9-125">Authorization</span></span>  | <span data-ttu-id="79df9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79df9-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79df9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="79df9-128">Request body</span></span>
<span data-ttu-id="79df9-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="79df9-129">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="79df9-130">属性</span><span class="sxs-lookup"><span data-stu-id="79df9-130">Property</span></span>     | <span data-ttu-id="79df9-131">类型</span><span class="sxs-lookup"><span data-stu-id="79df9-131">Type</span></span>   |<span data-ttu-id="79df9-132">说明</span><span class="sxs-lookup"><span data-stu-id="79df9-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79df9-133">values</span><span class="sxs-lookup"><span data-stu-id="79df9-133">values</span></span> | <span data-ttu-id="79df9-134">settingValue</span><span class="sxs-lookup"><span data-stu-id="79df9-134">settingValue</span></span> | <span data-ttu-id="79df9-p105">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="79df9-p105">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="79df9-138">响应</span><span class="sxs-lookup"><span data-stu-id="79df9-138">Response</span></span>

<span data-ttu-id="79df9-139">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="79df9-139">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79df9-140">示例</span><span class="sxs-lookup"><span data-stu-id="79df9-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79df9-141">请求</span><span class="sxs-lookup"><span data-stu-id="79df9-141">Request</span></span>
<span data-ttu-id="79df9-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79df9-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="79df9-143">响应</span><span class="sxs-lookup"><span data-stu-id="79df9-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->