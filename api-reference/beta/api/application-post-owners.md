---
title: 创建所有者
description: 使用此 API 创建一个新的所有者。
author: lleonard-msft
ms.openlocfilehash: 60aaec55b0cc2994bd9f001b1af81a64a6ddca14
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353443"
---
# <a name="create-owner"></a><span data-ttu-id="ea5be-103">创建所有者</span><span class="sxs-lookup"><span data-stu-id="ea5be-103">Create owner</span></span>

> <span data-ttu-id="ea5be-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea5be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea5be-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea5be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea5be-106">使用此 API 创建一个新的所有者。</span><span class="sxs-lookup"><span data-stu-id="ea5be-106">Use this API to create a new owner.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea5be-107">权限</span><span class="sxs-lookup"><span data-stu-id="ea5be-107">Permissions</span></span>
<span data-ttu-id="ea5be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea5be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea5be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea5be-110">Permission type</span></span>      | <span data-ttu-id="ea5be-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea5be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea5be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea5be-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ea5be-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea5be-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea5be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea5be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea5be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea5be-115">Not supported.</span></span>    |
|<span data-ttu-id="ea5be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea5be-116">Application</span></span> | <span data-ttu-id="ea5be-117">Application.ReadWrite.OwnedBy Directory.Read.All、 Application.ReadWrite.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea5be-117">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea5be-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea5be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="ea5be-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea5be-119">Request headers</span></span>
| <span data-ttu-id="ea5be-120">Name</span><span class="sxs-lookup"><span data-stu-id="ea5be-120">Name</span></span>       | <span data-ttu-id="ea5be-121">类型</span><span class="sxs-lookup"><span data-stu-id="ea5be-121">Type</span></span> | <span data-ttu-id="ea5be-122">说明</span><span class="sxs-lookup"><span data-stu-id="ea5be-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ea5be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea5be-123">Authorization</span></span>  | <span data-ttu-id="ea5be-124">string</span><span class="sxs-lookup"><span data-stu-id="ea5be-124">string</span></span>  | <span data-ttu-id="ea5be-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea5be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea5be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea5be-127">Request body</span></span>
<span data-ttu-id="ea5be-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea5be-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea5be-129">响应</span><span class="sxs-lookup"><span data-stu-id="ea5be-129">Response</span></span>

<span data-ttu-id="ea5be-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea5be-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea5be-131">示例</span><span class="sxs-lookup"><span data-stu-id="ea5be-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea5be-132">请求</span><span class="sxs-lookup"><span data-stu-id="ea5be-132">Request</span></span>
<span data-ttu-id="ea5be-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea5be-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="ea5be-134">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea5be-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ea5be-135">响应</span><span class="sxs-lookup"><span data-stu-id="ea5be-135">Response</span></span>
<span data-ttu-id="ea5be-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea5be-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->