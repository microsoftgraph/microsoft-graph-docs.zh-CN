---
title: 更新 inferenceclassificationoverride
description: '按指定内容更改替代的 **ClassifyAs** 字段。 '
localization_priority: Normal
ms.openlocfilehash: 5e1bdfa05f78c4be12a170f8dc27f32f7c5ccb55
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613969"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="348b0-103">更新 inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="348b0-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="348b0-104">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="348b0-104">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="348b0-105">不能在 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 示例中使用 PATCH 更改任何其他字段。</span><span class="sxs-lookup"><span data-stu-id="348b0-105">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="348b0-106">如果发件人的替代存在，并且发件人更改了他/她的显示名称，可以使用 [POST](inferenceclassification-post-overrides.md) 强制更新现有替代中的名称字段。</span><span class="sxs-lookup"><span data-stu-id="348b0-106">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="348b0-107">如果发件人的替代存在，并且发件人更改了他/她的 SMTP 地址，“更新”此发件人的替代的唯一方法是：[删除](inferenceclassificationoverride-delete.md) 现有替代，然后使用新的 SMTP 地址 [创建](inferenceclassification-post-overrides.md) 新替代。</span><span class="sxs-lookup"><span data-stu-id="348b0-107">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="348b0-108">权限</span><span class="sxs-lookup"><span data-stu-id="348b0-108">Permissions</span></span>
<span data-ttu-id="348b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="348b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="348b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="348b0-111">Permission type</span></span>      | <span data-ttu-id="348b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="348b0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="348b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="348b0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="348b0-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="348b0-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="348b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="348b0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="348b0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="348b0-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="348b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="348b0-117">Application</span></span> | <span data-ttu-id="348b0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="348b0-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="348b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="348b0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="348b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="348b0-120">Request headers</span></span>
| <span data-ttu-id="348b0-121">名称</span><span class="sxs-lookup"><span data-stu-id="348b0-121">Name</span></span>       | <span data-ttu-id="348b0-122">类型</span><span class="sxs-lookup"><span data-stu-id="348b0-122">Type</span></span> | <span data-ttu-id="348b0-123">说明</span><span class="sxs-lookup"><span data-stu-id="348b0-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="348b0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="348b0-124">Authorization</span></span>  | <span data-ttu-id="348b0-125">string</span><span class="sxs-lookup"><span data-stu-id="348b0-125">string</span></span>  | <span data-ttu-id="348b0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="348b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="348b0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="348b0-128">Content-Type</span></span> | <span data-ttu-id="348b0-129">string</span><span class="sxs-lookup"><span data-stu-id="348b0-129">string</span></span>  | <span data-ttu-id="348b0-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="348b0-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="348b0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="348b0-132">Request body</span></span>
<span data-ttu-id="348b0-p104">在请求正文中，提供 **classifyAs** 的新值。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="348b0-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="348b0-135">属性</span><span class="sxs-lookup"><span data-stu-id="348b0-135">Property</span></span>     | <span data-ttu-id="348b0-136">类型</span><span class="sxs-lookup"><span data-stu-id="348b0-136">Type</span></span>   |<span data-ttu-id="348b0-137">说明</span><span class="sxs-lookup"><span data-stu-id="348b0-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="348b0-138">classifyAs</span><span class="sxs-lookup"><span data-stu-id="348b0-138">classifyAs</span></span>|<span data-ttu-id="348b0-139">string</span><span class="sxs-lookup"><span data-stu-id="348b0-139">string</span></span>| <span data-ttu-id="348b0-140">指定来自特定发件人的传入邮件始终应如何分类。</span><span class="sxs-lookup"><span data-stu-id="348b0-140">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="348b0-141">可能的值为: `focused`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="348b0-141">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="348b0-142">响应</span><span class="sxs-lookup"><span data-stu-id="348b0-142">Response</span></span>

<span data-ttu-id="348b0-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="348b0-143">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="348b0-144">示例</span><span class="sxs-lookup"><span data-stu-id="348b0-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="348b0-145">请求</span><span class="sxs-lookup"><span data-stu-id="348b0-145">Request</span></span>
<span data-ttu-id="348b0-146">以下示例将 SMTP 地址 randiw@adatum.onmicrosoft.com 的替代从 `other` 更改为 `focused`。</span><span class="sxs-lookup"><span data-stu-id="348b0-146">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="348b0-147">响应</span><span class="sxs-lookup"><span data-stu-id="348b0-147">Response</span></span>
<span data-ttu-id="348b0-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="348b0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="348b0-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="348b0-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="348b0-152">语言</span><span class="sxs-lookup"><span data-stu-id="348b0-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_inferenceclassificationoverride-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="348b0-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="348b0-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_inferenceclassificationoverride-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
