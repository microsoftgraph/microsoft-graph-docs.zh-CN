---
title: 列表组设置
description: 检索组设置对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4699f58442f66dbff3bfa3e3913266776c7f4ac5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014522"
---
# <a name="list-group-settings"></a><span data-ttu-id="198e2-103">列表组设置</span><span class="sxs-lookup"><span data-stu-id="198e2-103">List group settings</span></span>

<span data-ttu-id="198e2-104">检索组设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="198e2-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="198e2-105">权限</span><span class="sxs-lookup"><span data-stu-id="198e2-105">Permissions</span></span>

<span data-ttu-id="198e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="198e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="198e2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="198e2-108">Permission type</span></span>      | <span data-ttu-id="198e2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="198e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="198e2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="198e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="198e2-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="198e2-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="198e2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="198e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="198e2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="198e2-113">Not supported.</span></span>    |
|<span data-ttu-id="198e2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="198e2-114">Application</span></span> | <span data-ttu-id="198e2-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="198e2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="198e2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="198e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="198e2-117">列出租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="198e2-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="198e2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="198e2-118">Optional query parameters</span></span>
<span data-ttu-id="198e2-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="198e2-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="198e2-120">**注意：** 不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="198e2-120">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="198e2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="198e2-121">Request headers</span></span>
| <span data-ttu-id="198e2-122">名称</span><span class="sxs-lookup"><span data-stu-id="198e2-122">Name</span></span> | <span data-ttu-id="198e2-123">说明</span><span class="sxs-lookup"><span data-stu-id="198e2-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="198e2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="198e2-124">Authorization</span></span>  | <span data-ttu-id="198e2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="198e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="198e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="198e2-127">Request body</span></span>
<span data-ttu-id="198e2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="198e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="198e2-129">响应</span><span class="sxs-lookup"><span data-stu-id="198e2-129">Response</span></span>

<span data-ttu-id="198e2-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[groupSetting](../resources/groupsetting.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="198e2-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="198e2-131">示例</span><span class="sxs-lookup"><span data-stu-id="198e2-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="198e2-132">请求</span><span class="sxs-lookup"><span data-stu-id="198e2-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="198e2-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="198e2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="198e2-134">C#</span><span class="sxs-lookup"><span data-stu-id="198e2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="198e2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="198e2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="198e2-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="198e2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="198e2-137">Java</span><span class="sxs-lookup"><span data-stu-id="198e2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="198e2-138">响应</span><span class="sxs-lookup"><span data-stu-id="198e2-138">Response</span></span>

<span data-ttu-id="198e2-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="198e2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
