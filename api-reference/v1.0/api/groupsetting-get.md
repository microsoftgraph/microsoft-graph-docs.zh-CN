---
title: 获取组设置
description: 检索特定组设置对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa78d40ae1d7434d5e0cba7fe9d8d117f8b8f900
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613291"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="b4f22-103">获取组设置</span><span class="sxs-lookup"><span data-stu-id="b4f22-103">Get a group setting</span></span>

<span data-ttu-id="b4f22-104">检索特定组设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4f22-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4f22-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4f22-105">Permissions</span></span>

<span data-ttu-id="b4f22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b4f22-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4f22-108">Permission type</span></span>      | <span data-ttu-id="b4f22-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4f22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4f22-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4f22-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4f22-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4f22-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4f22-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4f22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4f22-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4f22-113">Not supported.</span></span>    |
|<span data-ttu-id="b4f22-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4f22-114">Application</span></span> | <span data-ttu-id="b4f22-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f22-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4f22-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4f22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b4f22-117">获取特定的租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="b4f22-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4f22-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b4f22-118">Optional query parameters</span></span>
<span data-ttu-id="b4f22-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4f22-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="b4f22-120">注意：不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="b4f22-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4f22-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4f22-121">Request headers</span></span>
| <span data-ttu-id="b4f22-122">名称</span><span class="sxs-lookup"><span data-stu-id="b4f22-122">Name</span></span> | <span data-ttu-id="b4f22-123">说明</span><span class="sxs-lookup"><span data-stu-id="b4f22-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b4f22-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4f22-124">Authorization</span></span> | <span data-ttu-id="b4f22-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4f22-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4f22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4f22-127">Request body</span></span>

<span data-ttu-id="b4f22-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4f22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4f22-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4f22-129">Response</span></span>

<span data-ttu-id="b4f22-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[groupSetting](../resources/groupsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4f22-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4f22-131">示例</span><span class="sxs-lookup"><span data-stu-id="b4f22-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4f22-132">请求</span><span class="sxs-lookup"><span data-stu-id="b4f22-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="b4f22-133">响应</span><span class="sxs-lookup"><span data-stu-id="b4f22-133">Response</span></span>

<span data-ttu-id="b4f22-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4f22-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4f22-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b4f22-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4f22-137">语言</span><span class="sxs-lookup"><span data-stu-id="b4f22-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4f22-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4f22-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
