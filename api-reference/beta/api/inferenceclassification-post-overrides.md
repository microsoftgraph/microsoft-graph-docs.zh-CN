---
title: 创建 inferenceClassificationOverride
description: '为由 SMTP 地址标识的发件人创建重点收件箱覆盖。 将对来自该 SMTP 地址的未来邮件进行一致的分类 '
localization_priority: Normal
ms.openlocfilehash: 26524a50b56e49a7e28192124a94a52ad28ccd7c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592091"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="8ce3b-104">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="8ce3b-104">Create inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce3b-105">为由 SMTP 地址标识的发件人创建[重点收件箱](../resources/manage-focused-inbox.md)覆盖。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-105">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="8ce3b-106">将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-106">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="8ce3b-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="8ce3b-107">**Note**</span></span>

- <span data-ttu-id="8ce3b-108">如果已经存在具有相同 STMP 地址的替代，则用提供的值更新该替代的 **classifyAs** 和 **name** 字段。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="8ce3b-109">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="8ce3b-110">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ce3b-111">权限</span><span class="sxs-lookup"><span data-stu-id="8ce3b-111">Permissions</span></span>
<span data-ttu-id="8ce3b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ce3b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ce3b-114">Permission type</span></span>      | <span data-ttu-id="8ce3b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ce3b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ce3b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ce3b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8ce3b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ce3b-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ce3b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ce3b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ce3b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ce3b-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ce3b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ce3b-120">Application</span></span> | <span data-ttu-id="8ce3b-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ce3b-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ce3b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ce3b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="8ce3b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ce3b-123">Request headers</span></span>
| <span data-ttu-id="8ce3b-124">名称</span><span class="sxs-lookup"><span data-stu-id="8ce3b-124">Name</span></span>       | <span data-ttu-id="8ce3b-125">类型</span><span class="sxs-lookup"><span data-stu-id="8ce3b-125">Type</span></span> | <span data-ttu-id="8ce3b-126">说明</span><span class="sxs-lookup"><span data-stu-id="8ce3b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ce3b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ce3b-127">Authorization</span></span>  | <span data-ttu-id="8ce3b-128">string</span><span class="sxs-lookup"><span data-stu-id="8ce3b-128">string</span></span>  | <span data-ttu-id="8ce3b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ce3b-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ce3b-131">Content-Type</span></span> | <span data-ttu-id="8ce3b-132">string</span><span class="sxs-lookup"><span data-stu-id="8ce3b-132">string</span></span>  | <span data-ttu-id="8ce3b-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ce3b-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ce3b-135">Request body</span></span>
<span data-ttu-id="8ce3b-136">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8ce3b-137">响应</span><span class="sxs-lookup"><span data-stu-id="8ce3b-137">Response</span></span>

<span data-ttu-id="8ce3b-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ce3b-139">示例</span><span class="sxs-lookup"><span data-stu-id="8ce3b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ce3b-140">请求</span><span class="sxs-lookup"><span data-stu-id="8ce3b-140">Request</span></span>
<span data-ttu-id="8ce3b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8ce3b-142">响应</span><span class="sxs-lookup"><span data-stu-id="8ce3b-142">Response</span></span>
<span data-ttu-id="8ce3b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ce3b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8ce3b-146">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8ce3b-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8ce3b-147">语言</span><span class="sxs-lookup"><span data-stu-id="8ce3b-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_inferenceclassificationoverride_from_inferenceclassification-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ce3b-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ce3b-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_inferenceclassificationoverride_from_inferenceclassification-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/inferenceclassification-post-overrides.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/inferenceclassification-post-overrides.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
