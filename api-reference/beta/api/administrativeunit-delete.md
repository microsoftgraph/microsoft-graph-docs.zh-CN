---
title: 删除 administrativeUnit
description: 删除 administrativeUnit。
author: lleonard-msft
ms.openlocfilehash: 1ae08969f8faaa113f1bffa25a204f68a3340d03
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331435"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="b198e-103">删除 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b198e-103">Delete administrativeUnit</span></span>

> <span data-ttu-id="b198e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b198e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b198e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b198e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b198e-106">删除[administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="b198e-106">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b198e-107">权限</span><span class="sxs-lookup"><span data-stu-id="b198e-107">Permissions</span></span>
<span data-ttu-id="b198e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b198e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b198e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b198e-110">Permission type</span></span>      | <span data-ttu-id="b198e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b198e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b198e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b198e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b198e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b198e-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b198e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b198e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b198e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b198e-115">Not supported.</span></span>    |
|<span data-ttu-id="b198e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b198e-116">Application</span></span> | <span data-ttu-id="b198e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b198e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b198e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b198e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b198e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b198e-119">Request headers</span></span>
| <span data-ttu-id="b198e-120">Name</span><span class="sxs-lookup"><span data-stu-id="b198e-120">Name</span></span>       | <span data-ttu-id="b198e-121">说明</span><span class="sxs-lookup"><span data-stu-id="b198e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b198e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b198e-122">Authorization</span></span>  | <span data-ttu-id="b198e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b198e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b198e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b198e-125">Request body</span></span>
<span data-ttu-id="b198e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b198e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b198e-127">响应</span><span class="sxs-lookup"><span data-stu-id="b198e-127">Response</span></span>

<span data-ttu-id="b198e-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b198e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b198e-130">示例</span><span class="sxs-lookup"><span data-stu-id="b198e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b198e-131">请求</span><span class="sxs-lookup"><span data-stu-id="b198e-131">Request</span></span>
<span data-ttu-id="b198e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b198e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="b198e-133">响应</span><span class="sxs-lookup"><span data-stu-id="b198e-133">Response</span></span>
<span data-ttu-id="b198e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b198e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
