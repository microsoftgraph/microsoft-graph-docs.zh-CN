---
title: 列出组设置
description: 检索组设置对象的列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6db805374ce4783ff9d339f128efd7bc416ab161
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761309"
---
# <a name="list-group-settings"></a><span data-ttu-id="5bb2c-103">列出组设置</span><span class="sxs-lookup"><span data-stu-id="5bb2c-103">List group settings</span></span>

<span data-ttu-id="5bb2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bb2c-105">检索组设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bb2c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5bb2c-106">Permissions</span></span>

<span data-ttu-id="5bb2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5bb2c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bb2c-109">Permission type</span></span>      | <span data-ttu-id="5bb2c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bb2c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bb2c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bb2c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5bb2c-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5bb2c-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5bb2c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bb2c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bb2c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-114">Not supported.</span></span>    |
|<span data-ttu-id="5bb2c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bb2c-115">Application</span></span> | <span data-ttu-id="5bb2c-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb2c-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bb2c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bb2c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5bb2c-118">列出租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5bb2c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5bb2c-119">Optional query parameters</span></span>
<span data-ttu-id="5bb2c-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="5bb2c-121">**注意：** 不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bb2c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bb2c-122">Request headers</span></span>
| <span data-ttu-id="5bb2c-123">名称</span><span class="sxs-lookup"><span data-stu-id="5bb2c-123">Name</span></span> | <span data-ttu-id="5bb2c-124">说明</span><span class="sxs-lookup"><span data-stu-id="5bb2c-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="5bb2c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bb2c-125">Authorization</span></span>  | <span data-ttu-id="5bb2c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bb2c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bb2c-128">Request body</span></span>
<span data-ttu-id="5bb2c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bb2c-130">响应</span><span class="sxs-lookup"><span data-stu-id="5bb2c-130">Response</span></span>

<span data-ttu-id="5bb2c-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [groupSetting](../resources/groupsetting.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bb2c-132">示例</span><span class="sxs-lookup"><span data-stu-id="5bb2c-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5bb2c-133">请求</span><span class="sxs-lookup"><span data-stu-id="5bb2c-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5bb2c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb2c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="5bb2c-135">C#</span><span class="sxs-lookup"><span data-stu-id="5bb2c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bb2c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bb2c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bb2c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bb2c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bb2c-138">Java</span><span class="sxs-lookup"><span data-stu-id="5bb2c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5bb2c-139">响应</span><span class="sxs-lookup"><span data-stu-id="5bb2c-139">Response</span></span>

<span data-ttu-id="5bb2c-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bb2c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

