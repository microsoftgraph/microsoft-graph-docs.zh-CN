---
title: 在组中创建目录设置
description: 使用此 API 为组创建新的目录设置。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8f4d7e70311d40b762bf5fc683ff9fd4c509ba82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418713"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="f8745-103">在组中创建目录设置</span><span class="sxs-lookup"><span data-stu-id="f8745-103">Create a directory setting on groups</span></span>

<span data-ttu-id="f8745-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f8745-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8745-105">使用此 API 为组创建新的目录设置。</span><span class="sxs-lookup"><span data-stu-id="f8745-105">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8745-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8745-106">Permissions</span></span>
<span data-ttu-id="f8745-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8745-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8745-109">Permission type</span></span>      | <span data-ttu-id="f8745-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8745-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8745-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8745-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8745-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8745-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8745-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8745-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8745-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8745-114">Not supported.</span></span>    |
|<span data-ttu-id="f8745-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8745-115">Application</span></span> | <span data-ttu-id="f8745-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8745-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8745-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8745-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="f8745-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8745-118">Request headers</span></span>
| <span data-ttu-id="f8745-119">名称</span><span class="sxs-lookup"><span data-stu-id="f8745-119">Name</span></span>       | <span data-ttu-id="f8745-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8745-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8745-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8745-121">Authorization</span></span>  | <span data-ttu-id="f8745-122">持有者 <token>。</span><span class="sxs-lookup"><span data-stu-id="f8745-122">Bearer <token>.</span></span> <span data-ttu-id="f8745-123">必需</span><span class="sxs-lookup"><span data-stu-id="f8745-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8745-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8745-124">Request body</span></span>
<span data-ttu-id="f8745-125">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8745-125">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f8745-126">响应</span><span class="sxs-lookup"><span data-stu-id="f8745-126">Response</span></span>

<span data-ttu-id="f8745-127">如果成功，此方法在`201 Created`响应正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8745-127">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8745-128">示例</span><span class="sxs-lookup"><span data-stu-id="f8745-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8745-129">请求</span><span class="sxs-lookup"><span data-stu-id="f8745-129">Request</span></span>
<span data-ttu-id="f8745-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8745-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8745-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8745-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="f8745-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8745-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f8745-133">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8745-133">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f8745-134">响应</span><span class="sxs-lookup"><span data-stu-id="f8745-134">Response</span></span>
<span data-ttu-id="f8745-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8745-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
