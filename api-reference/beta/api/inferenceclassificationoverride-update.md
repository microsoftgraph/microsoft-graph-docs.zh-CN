---
title: 更新 inferenceClassificationOverride
description: '指定重写更改为中心的收件箱的**classifyAs**域。 '
ms.openlocfilehash: 696b3826bf09d3e0f706a3c3fdfba620e416ef22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048545"
---
# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="619f0-103">更新 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="619f0-103">Update inferenceClassificationOverride</span></span>

> <span data-ttu-id="619f0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="619f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="619f0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="619f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="619f0-106">指定重写更改[中心收件箱](../resources/manage-focused-inbox.md)的**classifyAs**域。</span><span class="sxs-lookup"><span data-stu-id="619f0-106">Change the **classifyAs** field of a [Focused Inbox](../resources/manage-focused-inbox.md) override as specified.</span></span> 

<span data-ttu-id="619f0-107">不能在 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 示例中使用 PATCH 更改任何其他字段。</span><span class="sxs-lookup"><span data-stu-id="619f0-107">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance.</span></span> 

<span data-ttu-id="619f0-108">如果发件人的替代存在，并且发件人更改了他/她的显示名称，可以使用 [POST](inferenceclassification-post-overrides.md) 强制更新现有替代中的名称字段。</span><span class="sxs-lookup"><span data-stu-id="619f0-108">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification-post-overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="619f0-109">如果发件人的替代存在，并且发件人更改了他/她的 SMTP 地址，“更新”此发件人的替代的唯一方法是：[删除](inferenceclassificationoverride-delete.md) 现有替代，然后使用新的 SMTP 地址 [创建](inferenceclassification-post-overrides.md) 新替代。</span><span class="sxs-lookup"><span data-stu-id="619f0-109">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride-delete.md) the existing override and [creating](inferenceclassification-post-overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="619f0-110">权限</span><span class="sxs-lookup"><span data-stu-id="619f0-110">Permissions</span></span>
<span data-ttu-id="619f0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="619f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="619f0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="619f0-113">Permission type</span></span>      | <span data-ttu-id="619f0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="619f0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="619f0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="619f0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="619f0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="619f0-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="619f0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="619f0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="619f0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="619f0-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="619f0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="619f0-119">Application</span></span> | <span data-ttu-id="619f0-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="619f0-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="619f0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="619f0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="619f0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="619f0-122">Request headers</span></span>
| <span data-ttu-id="619f0-123">名称</span><span class="sxs-lookup"><span data-stu-id="619f0-123">Name</span></span>       | <span data-ttu-id="619f0-124">类型</span><span class="sxs-lookup"><span data-stu-id="619f0-124">Type</span></span> | <span data-ttu-id="619f0-125">说明</span><span class="sxs-lookup"><span data-stu-id="619f0-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="619f0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="619f0-126">Authorization</span></span>  | <span data-ttu-id="619f0-127">string</span><span class="sxs-lookup"><span data-stu-id="619f0-127">string</span></span>  | <span data-ttu-id="619f0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="619f0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="619f0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="619f0-130">Content-Type</span></span> | <span data-ttu-id="619f0-131">string</span><span class="sxs-lookup"><span data-stu-id="619f0-131">string</span></span>  | <span data-ttu-id="619f0-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="619f0-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="619f0-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="619f0-134">Request body</span></span>
<span data-ttu-id="619f0-p105">在请求正文中，提供 **classifyAs** 的新值。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="619f0-p105">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="619f0-137">属性</span><span class="sxs-lookup"><span data-stu-id="619f0-137">Property</span></span>     | <span data-ttu-id="619f0-138">类型</span><span class="sxs-lookup"><span data-stu-id="619f0-138">Type</span></span>   |<span data-ttu-id="619f0-139">说明</span><span class="sxs-lookup"><span data-stu-id="619f0-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="619f0-140">classifyAs</span><span class="sxs-lookup"><span data-stu-id="619f0-140">classifyAs</span></span>|<span data-ttu-id="619f0-141">string</span><span class="sxs-lookup"><span data-stu-id="619f0-141">string</span></span>| <span data-ttu-id="619f0-p106">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="619f0-p106">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="619f0-144">响应</span><span class="sxs-lookup"><span data-stu-id="619f0-144">Response</span></span>

<span data-ttu-id="619f0-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="619f0-145">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="619f0-146">示例</span><span class="sxs-lookup"><span data-stu-id="619f0-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="619f0-147">请求</span><span class="sxs-lookup"><span data-stu-id="619f0-147">Request</span></span>
<span data-ttu-id="619f0-148">以下示例将 SMTP 地址 randiw@adatum.onmicrosoft.com 的替代从 `other` 更改为 `focused`。</span><span class="sxs-lookup"><span data-stu-id="619f0-148">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="619f0-149">响应</span><span class="sxs-lookup"><span data-stu-id="619f0-149">Response</span></span>
<span data-ttu-id="619f0-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="619f0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->