---
title: 创建 inferenceClassificationOverride
description: '创建由 SMTP 地址识别的发件人的替代。 将对来自该 SMTP 地址的未来邮件进行一致的分类 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 5fcb12edb24a106b39d19a89274353d1f8f953a0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372572"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="27ea6-104">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="27ea6-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="27ea6-p102">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="27ea6-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="27ea6-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="27ea6-107">**Note**</span></span>

- <span data-ttu-id="27ea6-108">如果已存在具有相同 SMTP 地址的替代, 则将使用所提供的值更新该替代的**classifyAs**和**name**字段。</span><span class="sxs-lookup"><span data-stu-id="27ea6-108">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="27ea6-109">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="27ea6-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="27ea6-110">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="27ea6-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="27ea6-111">权限</span><span class="sxs-lookup"><span data-stu-id="27ea6-111">Permissions</span></span>
<span data-ttu-id="27ea6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27ea6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27ea6-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="27ea6-114">Permission type</span></span>      | <span data-ttu-id="27ea6-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27ea6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27ea6-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27ea6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="27ea6-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27ea6-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="27ea6-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27ea6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27ea6-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27ea6-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="27ea6-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="27ea6-120">Application</span></span> | <span data-ttu-id="27ea6-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27ea6-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="27ea6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27ea6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="27ea6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="27ea6-123">Request headers</span></span>
| <span data-ttu-id="27ea6-124">名称</span><span class="sxs-lookup"><span data-stu-id="27ea6-124">Name</span></span>       | <span data-ttu-id="27ea6-125">类型</span><span class="sxs-lookup"><span data-stu-id="27ea6-125">Type</span></span> | <span data-ttu-id="27ea6-126">说明</span><span class="sxs-lookup"><span data-stu-id="27ea6-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27ea6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="27ea6-127">Authorization</span></span>  | <span data-ttu-id="27ea6-128">string</span><span class="sxs-lookup"><span data-stu-id="27ea6-128">string</span></span>  | <span data-ttu-id="27ea6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27ea6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27ea6-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27ea6-131">Content-Type</span></span> | <span data-ttu-id="27ea6-132">string</span><span class="sxs-lookup"><span data-stu-id="27ea6-132">string</span></span>  | <span data-ttu-id="27ea6-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="27ea6-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27ea6-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="27ea6-135">Request body</span></span>
<span data-ttu-id="27ea6-136">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27ea6-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27ea6-137">响应</span><span class="sxs-lookup"><span data-stu-id="27ea6-137">Response</span></span>

<span data-ttu-id="27ea6-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27ea6-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27ea6-139">示例</span><span class="sxs-lookup"><span data-stu-id="27ea6-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27ea6-140">请求</span><span class="sxs-lookup"><span data-stu-id="27ea6-140">Request</span></span>
<span data-ttu-id="27ea6-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27ea6-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27ea6-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="27ea6-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="27ea6-143">C#</span><span class="sxs-lookup"><span data-stu-id="27ea6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27ea6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27ea6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27ea6-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="27ea6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27ea6-146">Java</span><span class="sxs-lookup"><span data-stu-id="27ea6-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-inferenceclassificationoverride-from-inferenceclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="27ea6-147">响应</span><span class="sxs-lookup"><span data-stu-id="27ea6-147">Response</span></span>
<span data-ttu-id="27ea6-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27ea6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
