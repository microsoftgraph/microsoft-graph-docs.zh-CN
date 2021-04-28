---
title: 列出组设置
description: 检索组设置对象的列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d3a957e04db294cfc806e44c3ee6078cd9e54473
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039567"
---
# <a name="list-group-settings"></a><span data-ttu-id="770b3-103">列出组设置</span><span class="sxs-lookup"><span data-stu-id="770b3-103">List group settings</span></span>

<span data-ttu-id="770b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="770b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="770b3-105">检索组设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="770b3-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="770b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="770b3-106">Permissions</span></span>

<span data-ttu-id="770b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="770b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="770b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="770b3-109">Permission type</span></span>      | <span data-ttu-id="770b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="770b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="770b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="770b3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="770b3-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="770b3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="770b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="770b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="770b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="770b3-114">Not supported.</span></span>    |
|<span data-ttu-id="770b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="770b3-115">Application</span></span> | <span data-ttu-id="770b3-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="770b3-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="770b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="770b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="770b3-118">列出租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="770b3-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="770b3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="770b3-119">Optional query parameters</span></span>
<span data-ttu-id="770b3-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="770b3-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="770b3-121">**注意：** 不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="770b3-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="770b3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="770b3-122">Request headers</span></span>
| <span data-ttu-id="770b3-123">名称</span><span class="sxs-lookup"><span data-stu-id="770b3-123">Name</span></span> | <span data-ttu-id="770b3-124">说明</span><span class="sxs-lookup"><span data-stu-id="770b3-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="770b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="770b3-125">Authorization</span></span>  | <span data-ttu-id="770b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="770b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="770b3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="770b3-128">Request body</span></span>
<span data-ttu-id="770b3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="770b3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="770b3-130">响应</span><span class="sxs-lookup"><span data-stu-id="770b3-130">Response</span></span>

<span data-ttu-id="770b3-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [groupSetting](../resources/groupsetting.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="770b3-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="770b3-132">示例</span><span class="sxs-lookup"><span data-stu-id="770b3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="770b3-133">请求</span><span class="sxs-lookup"><span data-stu-id="770b3-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="770b3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="770b3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="770b3-135">C#</span><span class="sxs-lookup"><span data-stu-id="770b3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="770b3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="770b3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="770b3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="770b3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="770b3-138">Java</span><span class="sxs-lookup"><span data-stu-id="770b3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="770b3-139">响应</span><span class="sxs-lookup"><span data-stu-id="770b3-139">Response</span></span>

<span data-ttu-id="770b3-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="770b3-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

