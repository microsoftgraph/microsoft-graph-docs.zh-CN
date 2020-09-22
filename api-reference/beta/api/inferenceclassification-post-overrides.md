---
title: 创建 inferenceClassificationOverride
description: '创建由 SMTP 地址识别的发件人的重点收件箱替代。 将对来自该 SMTP 地址的未来邮件进行一致的分类 '
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: ''
ms.openlocfilehash: fc966d3bf067e5c8a397c828733fff5152e50475
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990653"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="4be8a-104">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4be8a-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="4be8a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4be8a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be8a-106">为由 SMTP 地址标识的发件人创建 [重点收件箱](../resources/manage-focused-inbox.md) 覆盖。</span><span class="sxs-lookup"><span data-stu-id="4be8a-106">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="4be8a-107">将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="4be8a-107">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="4be8a-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="4be8a-108">**Note**</span></span>

- <span data-ttu-id="4be8a-109">如果已存在具有相同 SMTP 地址的替代，则将使用所提供的值更新该替代的 **classifyAs** 和 **name** 字段。</span><span class="sxs-lookup"><span data-stu-id="4be8a-109">If an override already exists with the same SMTP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="4be8a-110">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="4be8a-110">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="4be8a-111">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="4be8a-111">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be8a-112">权限</span><span class="sxs-lookup"><span data-stu-id="4be8a-112">Permissions</span></span>
<span data-ttu-id="4be8a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4be8a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be8a-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="4be8a-115">Permission type</span></span>      | <span data-ttu-id="4be8a-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4be8a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be8a-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4be8a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4be8a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4be8a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4be8a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4be8a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be8a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4be8a-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4be8a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="4be8a-121">Application</span></span> | <span data-ttu-id="4be8a-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4be8a-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be8a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4be8a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="4be8a-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4be8a-124">Request headers</span></span>
| <span data-ttu-id="4be8a-125">名称</span><span class="sxs-lookup"><span data-stu-id="4be8a-125">Name</span></span>       | <span data-ttu-id="4be8a-126">类型</span><span class="sxs-lookup"><span data-stu-id="4be8a-126">Type</span></span> | <span data-ttu-id="4be8a-127">说明</span><span class="sxs-lookup"><span data-stu-id="4be8a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4be8a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="4be8a-128">Authorization</span></span>  | <span data-ttu-id="4be8a-129">string</span><span class="sxs-lookup"><span data-stu-id="4be8a-129">string</span></span>  | <span data-ttu-id="4be8a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4be8a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4be8a-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4be8a-132">Content-Type</span></span> | <span data-ttu-id="4be8a-133">string</span><span class="sxs-lookup"><span data-stu-id="4be8a-133">string</span></span>  | <span data-ttu-id="4be8a-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="4be8a-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4be8a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="4be8a-136">Request body</span></span>
<span data-ttu-id="4be8a-137">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4be8a-137">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4be8a-138">响应</span><span class="sxs-lookup"><span data-stu-id="4be8a-138">Response</span></span>

<span data-ttu-id="4be8a-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4be8a-139">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be8a-140">示例</span><span class="sxs-lookup"><span data-stu-id="4be8a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4be8a-141">请求</span><span class="sxs-lookup"><span data-stu-id="4be8a-141">Request</span></span>
<span data-ttu-id="4be8a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4be8a-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4be8a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4be8a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/beta/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4be8a-144">C#</span><span class="sxs-lookup"><span data-stu-id="4be8a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-inferenceclassificationoverride-from-inferenceclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4be8a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4be8a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-inferenceclassificationoverride-from-inferenceclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4be8a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4be8a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-inferenceclassificationoverride-from-inferenceclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4be8a-147">响应</span><span class="sxs-lookup"><span data-stu-id="4be8a-147">Response</span></span>
<span data-ttu-id="4be8a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4be8a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


