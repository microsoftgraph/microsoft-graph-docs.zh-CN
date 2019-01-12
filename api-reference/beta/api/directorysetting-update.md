---
title: 更新目录设置
description: 更新特定目录设置对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e7228402069e4803f108833abfe08dc84d1082c9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935890"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="aa660-103">更新目录设置</span><span class="sxs-lookup"><span data-stu-id="aa660-103">Update a directory setting</span></span>

> <span data-ttu-id="aa660-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa660-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa660-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa660-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa660-106">更新特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa660-106">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="aa660-107">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="aa660-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="aa660-108">此 API 的 /v1.0 版本已被重命名为*更新 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="aa660-108">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa660-109">权限</span><span class="sxs-lookup"><span data-stu-id="aa660-109">Permissions</span></span>
<span data-ttu-id="aa660-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa660-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa660-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa660-112">Permission type</span></span>      | <span data-ttu-id="aa660-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa660-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa660-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa660-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aa660-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa660-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa660-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa660-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa660-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa660-117">Not supported.</span></span>    |
|<span data-ttu-id="aa660-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa660-118">Application</span></span> | <span data-ttu-id="aa660-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa660-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa660-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa660-120">HTTP request</span></span>
<span data-ttu-id="aa660-121"><!-- { "blockType": "ignored" } -->更新租户范围内或组的特定设置。</span><span class="sxs-lookup"><span data-stu-id="aa660-121"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="aa660-122">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="aa660-122">Optional request headers</span></span>
| <span data-ttu-id="aa660-123">名称</span><span class="sxs-lookup"><span data-stu-id="aa660-123">Name</span></span>       | <span data-ttu-id="aa660-124">说明</span><span class="sxs-lookup"><span data-stu-id="aa660-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aa660-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa660-125">Authorization</span></span>  | <span data-ttu-id="aa660-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa660-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa660-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa660-128">Request body</span></span>
<span data-ttu-id="aa660-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="aa660-129">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="aa660-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa660-130">Property</span></span>     | <span data-ttu-id="aa660-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa660-131">Type</span></span>   |<span data-ttu-id="aa660-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa660-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa660-133">values</span><span class="sxs-lookup"><span data-stu-id="aa660-133">values</span></span> | <span data-ttu-id="aa660-134">settingValue</span><span class="sxs-lookup"><span data-stu-id="aa660-134">settingValue</span></span> | <span data-ttu-id="aa660-p105">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="aa660-p105">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="aa660-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa660-138">Response</span></span>

<span data-ttu-id="aa660-139">如果成功，此方法返回 `204 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aa660-139">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa660-140">示例</span><span class="sxs-lookup"><span data-stu-id="aa660-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa660-141">请求</span><span class="sxs-lookup"><span data-stu-id="aa660-141">Request</span></span>
<span data-ttu-id="aa660-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa660-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="aa660-143">响应</span><span class="sxs-lookup"><span data-stu-id="aa660-143">Response</span></span>
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
