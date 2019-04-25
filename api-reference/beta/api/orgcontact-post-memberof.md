---
title: 创建 memberOf
description: 使用此 API 创建新的 memberOf。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 466074d2d23dc4b991c8c153252028587fd5afcc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539708"
---
# <a name="create-memberof"></a><span data-ttu-id="0e10c-103">创建 memberOf</span><span class="sxs-lookup"><span data-stu-id="0e10c-103">Create memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e10c-104">使用此 API 创建新的 memberOf。</span><span class="sxs-lookup"><span data-stu-id="0e10c-104">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e10c-105">权限</span><span class="sxs-lookup"><span data-stu-id="0e10c-105">Permissions</span></span>
<span data-ttu-id="0e10c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e10c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e10c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e10c-108">Permission type</span></span>      | <span data-ttu-id="0e10c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e10c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e10c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e10c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e10c-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e10c-111">Not supported.</span></span>    |
|<span data-ttu-id="0e10c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e10c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e10c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e10c-113">Not supported.</span></span>    |
|<span data-ttu-id="0e10c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e10c-114">Application</span></span> | <span data-ttu-id="0e10c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e10c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e10c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e10c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="0e10c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e10c-117">Request headers</span></span>
| <span data-ttu-id="0e10c-118">名称</span><span class="sxs-lookup"><span data-stu-id="0e10c-118">Name</span></span>       | <span data-ttu-id="0e10c-119">类型</span><span class="sxs-lookup"><span data-stu-id="0e10c-119">Type</span></span> | <span data-ttu-id="0e10c-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e10c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e10c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e10c-121">Authorization</span></span>  | <span data-ttu-id="0e10c-122">string</span><span class="sxs-lookup"><span data-stu-id="0e10c-122">string</span></span>  | <span data-ttu-id="0e10c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e10c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e10c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e10c-125">Request body</span></span>
<span data-ttu-id="0e10c-126">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e10c-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0e10c-127">响应</span><span class="sxs-lookup"><span data-stu-id="0e10c-127">Response</span></span>

<span data-ttu-id="0e10c-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e10c-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e10c-129">示例</span><span class="sxs-lookup"><span data-stu-id="0e10c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e10c-130">请求</span><span class="sxs-lookup"><span data-stu-id="0e10c-130">Request</span></span>
<span data-ttu-id="0e10c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e10c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="0e10c-132">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e10c-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0e10c-133">响应</span><span class="sxs-lookup"><span data-stu-id="0e10c-133">Response</span></span>
<span data-ttu-id="0e10c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e10c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-post-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
