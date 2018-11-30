---
title: 创建 inferenceClassificationOverride
description: '创建发件人的 SMTP 地址被标识为中心的收件箱覆盖。 今后来自该 SMTP 地址的邮件将被始终分类 '
ms.openlocfilehash: e15793bc8c7012628659144bd503bd8cf979ef61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044263"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="7617b-104">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="7617b-104">Create inferenceClassificationOverride</span></span>

> <span data-ttu-id="7617b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7617b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7617b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7617b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7617b-107">创建发件人的 SMTP 地址被标识为[中心的收件箱](../resources/manage-focused-inbox.md)覆盖。</span><span class="sxs-lookup"><span data-stu-id="7617b-107">Create a [Focused Inbox](../resources/manage-focused-inbox.md) override for a sender identified by an SMTP address.</span></span> <span data-ttu-id="7617b-108">从邮件未来一致地进行分类 SMTP 地址重写中指定。</span><span class="sxs-lookup"><span data-stu-id="7617b-108">Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="7617b-109">**注意**</span><span class="sxs-lookup"><span data-stu-id="7617b-109">**Note**</span></span>

- <span data-ttu-id="7617b-110">如果已经存在具有相同 STMP 地址的替代，则用提供的值更新该替代的 **classifyAs** 和 **name** 字段。</span><span class="sxs-lookup"><span data-stu-id="7617b-110">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="7617b-111">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="7617b-111">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="7617b-112">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="7617b-112">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="7617b-113">权限</span><span class="sxs-lookup"><span data-stu-id="7617b-113">Permissions</span></span>
<span data-ttu-id="7617b-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7617b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7617b-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="7617b-116">Permission type</span></span>      | <span data-ttu-id="7617b-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7617b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7617b-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7617b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7617b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7617b-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7617b-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7617b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7617b-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7617b-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7617b-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="7617b-122">Application</span></span> | <span data-ttu-id="7617b-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7617b-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7617b-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7617b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="7617b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7617b-125">Request headers</span></span>
| <span data-ttu-id="7617b-126">名称</span><span class="sxs-lookup"><span data-stu-id="7617b-126">Name</span></span>       | <span data-ttu-id="7617b-127">类型</span><span class="sxs-lookup"><span data-stu-id="7617b-127">Type</span></span> | <span data-ttu-id="7617b-128">说明</span><span class="sxs-lookup"><span data-stu-id="7617b-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7617b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7617b-129">Authorization</span></span>  | <span data-ttu-id="7617b-130">string</span><span class="sxs-lookup"><span data-stu-id="7617b-130">string</span></span>  | <span data-ttu-id="7617b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7617b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7617b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7617b-133">Content-Type</span></span> | <span data-ttu-id="7617b-134">string</span><span class="sxs-lookup"><span data-stu-id="7617b-134">string</span></span>  | <span data-ttu-id="7617b-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="7617b-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7617b-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="7617b-137">Request body</span></span>
<span data-ttu-id="7617b-138">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7617b-138">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7617b-139">响应</span><span class="sxs-lookup"><span data-stu-id="7617b-139">Response</span></span>

<span data-ttu-id="7617b-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7617b-140">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7617b-141">示例</span><span class="sxs-lookup"><span data-stu-id="7617b-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7617b-142">请求</span><span class="sxs-lookup"><span data-stu-id="7617b-142">Request</span></span>
<span data-ttu-id="7617b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7617b-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7617b-144">响应</span><span class="sxs-lookup"><span data-stu-id="7617b-144">Response</span></span>
<span data-ttu-id="7617b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7617b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->