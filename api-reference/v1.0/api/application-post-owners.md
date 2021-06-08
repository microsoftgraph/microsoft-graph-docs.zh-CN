---
title: 添加所有者
description: 向应用程序添加所有者。
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5640b2488ccabc24f512e823924b7be0e3df7342
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787980"
---
# <a name="add-owner"></a><span data-ttu-id="80df1-103">添加所有者</span><span class="sxs-lookup"><span data-stu-id="80df1-103">Add owner</span></span>

<span data-ttu-id="80df1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80df1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80df1-105">通过发布到所有者 [集合](../resources/application.md) 将所有者添加到应用程序。</span><span class="sxs-lookup"><span data-stu-id="80df1-105">Add an owner to an [application](../resources/application.md) by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="80df1-106">权限</span><span class="sxs-lookup"><span data-stu-id="80df1-106">Permissions</span></span>
<span data-ttu-id="80df1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80df1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80df1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80df1-109">Permission type</span></span>      | <span data-ttu-id="80df1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80df1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80df1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80df1-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="80df1-112">Application.ReadWrite.All 和 Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80df1-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80df1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80df1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80df1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80df1-114">Not supported.</span></span>    |
|<span data-ttu-id="80df1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80df1-115">Application</span></span> | <span data-ttu-id="80df1-116">Application.ReadWrite.OwnedBy 和 Directory.Read.All、Application.ReadWrite.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="80df1-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

> <span data-ttu-id="80df1-117">**注意\*\*\*\*：Application.ReadWrite.OwnedBy** 不足以添加其他所有者。</span><span class="sxs-lookup"><span data-stu-id="80df1-117">**Note:** **Application.ReadWrite.OwnedBy** will not be sufficient to add another owner.</span></span> <span data-ttu-id="80df1-118">也同意 **Application.ReadWrite.All。**</span><span class="sxs-lookup"><span data-stu-id="80df1-118">Consent also to **Application.ReadWrite.All**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="80df1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80df1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="80df1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80df1-120">Request headers</span></span>
| <span data-ttu-id="80df1-121">名称</span><span class="sxs-lookup"><span data-stu-id="80df1-121">Name</span></span> | <span data-ttu-id="80df1-122">说明</span><span class="sxs-lookup"><span data-stu-id="80df1-122">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="80df1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80df1-123">Authorization</span></span> | <span data-ttu-id="80df1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80df1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80df1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="80df1-126">Request body</span></span>
<span data-ttu-id="80df1-127">在请求正文中，提供要分配为所有者的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="80df1-127">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="80df1-128">响应</span><span class="sxs-lookup"><span data-stu-id="80df1-128">Response</span></span>

<span data-ttu-id="80df1-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="80df1-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80df1-130">示例</span><span class="sxs-lookup"><span data-stu-id="80df1-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="80df1-131">请求</span><span class="sxs-lookup"><span data-stu-id="80df1-131">Request</span></span>
<span data-ttu-id="80df1-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="80df1-132">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="80df1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80df1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="80df1-134">C#</span><span class="sxs-lookup"><span data-stu-id="80df1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80df1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80df1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80df1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80df1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80df1-137">Java</span><span class="sxs-lookup"><span data-stu-id="80df1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80df1-138">响应</span><span class="sxs-lookup"><span data-stu-id="80df1-138">Response</span></span>

<span data-ttu-id="80df1-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80df1-139">The following is an example of the response.</span></span>

><span data-ttu-id="80df1-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80df1-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

