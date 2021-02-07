---
title: 更新 inferenceclassificationoverride
description: '按指定内容更改替代的 **ClassifyAs** 字段。 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 60625066f8da1c8ad0effeaad33a55a4b32dd81b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135189"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="08454-103">更新 inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="08454-103">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="08454-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08454-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08454-105">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="08454-105">Change the **classifyAs** field of an override as specified.</span></span>

<span data-ttu-id="08454-106">不能在 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 示例中使用 PATCH 更改任何其他字段。</span><span class="sxs-lookup"><span data-stu-id="08454-106">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span>

<span data-ttu-id="08454-107">如果发件人的替代存在，并且发件人更改了他/她的显示名称，可以使用 [POST](inferenceclassification-post-overrides.md) 强制更新现有替代中的名称字段。</span><span class="sxs-lookup"><span data-stu-id="08454-107">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="08454-108">如果发件人的替代存在，并且发件人更改了他/她的 SMTP 地址，“更新”此发件人的替代的唯一方法是：[删除](inferenceclassificationoverride-delete.md) 现有替代，然后使用新的 SMTP 地址 [创建](inferenceclassification-post-overrides.md) 新替代。</span><span class="sxs-lookup"><span data-stu-id="08454-108">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="08454-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="08454-109">Permissions</span></span>
<span data-ttu-id="08454-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08454-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="08454-112">Permission type</span></span>      | <span data-ttu-id="08454-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08454-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08454-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08454-114">Delegated (work or school account)</span></span> | <span data-ttu-id="08454-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08454-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="08454-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08454-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08454-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08454-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="08454-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="08454-118">Application</span></span> | <span data-ttu-id="08454-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08454-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="08454-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08454-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="08454-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="08454-121">Request headers</span></span>
| <span data-ttu-id="08454-122">名称</span><span class="sxs-lookup"><span data-stu-id="08454-122">Name</span></span>       | <span data-ttu-id="08454-123">类型</span><span class="sxs-lookup"><span data-stu-id="08454-123">Type</span></span> | <span data-ttu-id="08454-124">说明</span><span class="sxs-lookup"><span data-stu-id="08454-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08454-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08454-125">Authorization</span></span>  | <span data-ttu-id="08454-126">string</span><span class="sxs-lookup"><span data-stu-id="08454-126">string</span></span>  | <span data-ttu-id="08454-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08454-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08454-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08454-129">Content-Type</span></span> | <span data-ttu-id="08454-130">string</span><span class="sxs-lookup"><span data-stu-id="08454-130">string</span></span>  | <span data-ttu-id="08454-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="08454-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08454-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="08454-133">Request body</span></span>
<span data-ttu-id="08454-p104">在请求正文中，提供 **classifyAs** 的新值。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="08454-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="08454-136">属性</span><span class="sxs-lookup"><span data-stu-id="08454-136">Property</span></span>     | <span data-ttu-id="08454-137">类型</span><span class="sxs-lookup"><span data-stu-id="08454-137">Type</span></span>   |<span data-ttu-id="08454-138">说明</span><span class="sxs-lookup"><span data-stu-id="08454-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08454-139">classifyAs</span><span class="sxs-lookup"><span data-stu-id="08454-139">classifyAs</span></span>|<span data-ttu-id="08454-140">string</span><span class="sxs-lookup"><span data-stu-id="08454-140">string</span></span>| <span data-ttu-id="08454-141">指定来自特定发件人的传入邮件始终应如何分类。</span><span class="sxs-lookup"><span data-stu-id="08454-141">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="08454-142">可能的值是： `focused` `other` 。</span><span class="sxs-lookup"><span data-stu-id="08454-142">The possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="08454-143">响应</span><span class="sxs-lookup"><span data-stu-id="08454-143">Response</span></span>

<span data-ttu-id="08454-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08454-144">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08454-145">示例</span><span class="sxs-lookup"><span data-stu-id="08454-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08454-146">请求</span><span class="sxs-lookup"><span data-stu-id="08454-146">Request</span></span>
<span data-ttu-id="08454-147">以下示例将 SMTP 地址 randiw@adatum.onmicrosoft.com 的替代从 `other` 更改为 `focused`。</span><span class="sxs-lookup"><span data-stu-id="08454-147">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>


# <a name="http"></a>[<span data-ttu-id="08454-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="08454-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08454-149">C#</span><span class="sxs-lookup"><span data-stu-id="08454-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08454-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08454-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08454-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08454-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08454-152">Java</span><span class="sxs-lookup"><span data-stu-id="08454-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="08454-153">响应</span><span class="sxs-lookup"><span data-stu-id="08454-153">Response</span></span>
<span data-ttu-id="08454-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08454-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

