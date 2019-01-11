---
title: 删除 administrativeUnit
description: 删除 administrativeUnit。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 7c90fda4bdcbb6a431dbcb4caa6a50a130c7f78b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860051"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="37262-103">删除 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="37262-103">Delete administrativeUnit</span></span>

> <span data-ttu-id="37262-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="37262-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37262-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37262-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37262-106">删除[administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="37262-106">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37262-107">权限</span><span class="sxs-lookup"><span data-stu-id="37262-107">Permissions</span></span>
<span data-ttu-id="37262-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37262-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="37262-110">Permission type</span></span>      | <span data-ttu-id="37262-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37262-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37262-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37262-112">Delegated (work or school account)</span></span> | <span data-ttu-id="37262-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37262-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37262-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37262-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37262-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="37262-115">Not supported.</span></span>    |
|<span data-ttu-id="37262-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="37262-116">Application</span></span> | <span data-ttu-id="37262-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="37262-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37262-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37262-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="37262-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="37262-119">Request headers</span></span>
| <span data-ttu-id="37262-120">名称</span><span class="sxs-lookup"><span data-stu-id="37262-120">Name</span></span>       | <span data-ttu-id="37262-121">说明</span><span class="sxs-lookup"><span data-stu-id="37262-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37262-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37262-122">Authorization</span></span>  | <span data-ttu-id="37262-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37262-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37262-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="37262-125">Request body</span></span>
<span data-ttu-id="37262-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37262-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37262-127">响应</span><span class="sxs-lookup"><span data-stu-id="37262-127">Response</span></span>

<span data-ttu-id="37262-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="37262-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37262-130">示例</span><span class="sxs-lookup"><span data-stu-id="37262-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37262-131">请求</span><span class="sxs-lookup"><span data-stu-id="37262-131">Request</span></span>
<span data-ttu-id="37262-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37262-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="37262-133">响应</span><span class="sxs-lookup"><span data-stu-id="37262-133">Response</span></span>
<span data-ttu-id="37262-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37262-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
