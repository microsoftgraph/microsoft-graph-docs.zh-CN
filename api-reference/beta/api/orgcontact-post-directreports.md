---
title: 创建 directReport
description: 使用此 API 创建新 directReport。
localization_priority: Normal
ms.openlocfilehash: 8119ea6972f1ea5b4e94e68ff4acd0dc8771c99f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862557"
---
# <a name="create-directreport"></a><span data-ttu-id="46341-103">创建 directReport</span><span class="sxs-lookup"><span data-stu-id="46341-103">Create directReport</span></span>

> <span data-ttu-id="46341-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="46341-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46341-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="46341-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46341-106">使用此 API 创建新 directReport。</span><span class="sxs-lookup"><span data-stu-id="46341-106">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="46341-107">权限</span><span class="sxs-lookup"><span data-stu-id="46341-107">Permissions</span></span>
<span data-ttu-id="46341-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46341-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46341-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="46341-110">Permission type</span></span>      | <span data-ttu-id="46341-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46341-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46341-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46341-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46341-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="46341-113">Not supported.</span></span>    |
|<span data-ttu-id="46341-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46341-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46341-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46341-115">Not supported.</span></span>    |
|<span data-ttu-id="46341-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="46341-116">Application</span></span> | <span data-ttu-id="46341-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="46341-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46341-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46341-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="46341-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="46341-119">Request headers</span></span>
| <span data-ttu-id="46341-120">名称</span><span class="sxs-lookup"><span data-stu-id="46341-120">Name</span></span>       | <span data-ttu-id="46341-121">类型</span><span class="sxs-lookup"><span data-stu-id="46341-121">Type</span></span> | <span data-ttu-id="46341-122">说明</span><span class="sxs-lookup"><span data-stu-id="46341-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46341-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46341-123">Authorization</span></span>  | <span data-ttu-id="46341-124">string</span><span class="sxs-lookup"><span data-stu-id="46341-124">string</span></span>  | <span data-ttu-id="46341-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46341-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46341-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46341-127">Request body</span></span>
<span data-ttu-id="46341-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46341-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="46341-129">响应</span><span class="sxs-lookup"><span data-stu-id="46341-129">Response</span></span>

<span data-ttu-id="46341-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46341-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46341-131">示例</span><span class="sxs-lookup"><span data-stu-id="46341-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46341-132">请求</span><span class="sxs-lookup"><span data-stu-id="46341-132">Request</span></span>
<span data-ttu-id="46341-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46341-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="46341-134">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46341-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="46341-135">响应</span><span class="sxs-lookup"><span data-stu-id="46341-135">Response</span></span>
<span data-ttu-id="46341-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46341-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
