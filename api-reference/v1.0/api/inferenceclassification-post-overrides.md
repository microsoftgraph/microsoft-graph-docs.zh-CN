---
title: 创建 inferenceClassificationOverride
description: '创建由 SMTP 地址识别的发件人的替代。 来自该 SMTP 地址的未来邮件将一致分类 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6e3ec52690c605dd9c4ab6ea9cda7eb090650dd3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133866"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="e3545-104">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e3545-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="e3545-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3545-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3545-p102">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="e3545-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="e3545-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="e3545-108">**Note**</span></span>

- <span data-ttu-id="e3545-109">如果已存在同一 SMTP 地址的覆盖，则使用所提供的值更新该覆盖的 **分类** 和名称字段。</span><span class="sxs-lookup"><span data-stu-id="e3545-109">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="e3545-110">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="e3545-110">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="e3545-111">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="e3545-111">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3545-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3545-112">Permissions</span></span>
<span data-ttu-id="e3545-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3545-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3545-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3545-115">Permission type</span></span>      | <span data-ttu-id="e3545-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3545-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3545-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3545-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e3545-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3545-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e3545-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3545-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3545-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3545-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e3545-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3545-121">Application</span></span> | <span data-ttu-id="e3545-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3545-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3545-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3545-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="e3545-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3545-124">Request headers</span></span>
| <span data-ttu-id="e3545-125">名称</span><span class="sxs-lookup"><span data-stu-id="e3545-125">Name</span></span>       | <span data-ttu-id="e3545-126">类型</span><span class="sxs-lookup"><span data-stu-id="e3545-126">Type</span></span> | <span data-ttu-id="e3545-127">说明</span><span class="sxs-lookup"><span data-stu-id="e3545-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3545-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3545-128">Authorization</span></span>  | <span data-ttu-id="e3545-129">string</span><span class="sxs-lookup"><span data-stu-id="e3545-129">string</span></span>  | <span data-ttu-id="e3545-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3545-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3545-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3545-132">Content-Type</span></span> | <span data-ttu-id="e3545-133">string</span><span class="sxs-lookup"><span data-stu-id="e3545-133">string</span></span>  | <span data-ttu-id="e3545-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="e3545-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3545-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3545-136">Request body</span></span>
<span data-ttu-id="e3545-137">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3545-137">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e3545-138">响应</span><span class="sxs-lookup"><span data-stu-id="e3545-138">Response</span></span>

<span data-ttu-id="e3545-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3545-139">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3545-140">示例</span><span class="sxs-lookup"><span data-stu-id="e3545-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3545-141">请求</span><span class="sxs-lookup"><span data-stu-id="e3545-141">Request</span></span>
<span data-ttu-id="e3545-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3545-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3545-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3545-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e3545-144">C#</span><span class="sxs-lookup"><span data-stu-id="e3545-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3545-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3545-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3545-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3545-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3545-147">Java</span><span class="sxs-lookup"><span data-stu-id="e3545-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3545-148">响应</span><span class="sxs-lookup"><span data-stu-id="e3545-148">Response</span></span>
<span data-ttu-id="e3545-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3545-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

