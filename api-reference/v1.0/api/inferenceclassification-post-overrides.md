---
title: 创建 inferenceClassificationOverride
description: '创建由 SMTP 地址识别的发件人的替代。 将对来自该 SMTP 地址的未来邮件进行一致的分类 '
localization_priority: Normal
ms.openlocfilehash: 37648d699d4d54b2995af6bf847347c6537a414d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577621"
---
# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="92494-104">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="92494-104">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="92494-p102">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="92494-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="92494-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="92494-107">**Note**</span></span>

- <span data-ttu-id="92494-108">如果已经存在具有相同 STMP 地址的替代，则用提供的值更新该替代的 **classifyAs** 和 **name** 字段。</span><span class="sxs-lookup"><span data-stu-id="92494-108">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="92494-109">基于唯一发件人的 SMTP 地址，邮箱支持的最大替代数目为 1000 个。</span><span class="sxs-lookup"><span data-stu-id="92494-109">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="92494-110">POST 操作仅支持一次创建一个替代。</span><span class="sxs-lookup"><span data-stu-id="92494-110">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="92494-111">权限</span><span class="sxs-lookup"><span data-stu-id="92494-111">Permissions</span></span>
<span data-ttu-id="92494-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92494-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92494-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="92494-114">Permission type</span></span>      | <span data-ttu-id="92494-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92494-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92494-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92494-116">Delegated (work or school account)</span></span> | <span data-ttu-id="92494-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92494-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="92494-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92494-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92494-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92494-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="92494-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="92494-120">Application</span></span> | <span data-ttu-id="92494-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92494-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92494-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92494-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="92494-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="92494-123">Request headers</span></span>
| <span data-ttu-id="92494-124">名称</span><span class="sxs-lookup"><span data-stu-id="92494-124">Name</span></span>       | <span data-ttu-id="92494-125">类型</span><span class="sxs-lookup"><span data-stu-id="92494-125">Type</span></span> | <span data-ttu-id="92494-126">说明</span><span class="sxs-lookup"><span data-stu-id="92494-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="92494-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="92494-127">Authorization</span></span>  | <span data-ttu-id="92494-128">string</span><span class="sxs-lookup"><span data-stu-id="92494-128">string</span></span>  | <span data-ttu-id="92494-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92494-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92494-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92494-131">Content-Type</span></span> | <span data-ttu-id="92494-132">string</span><span class="sxs-lookup"><span data-stu-id="92494-132">string</span></span>  | <span data-ttu-id="92494-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="92494-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92494-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="92494-135">Request body</span></span>
<span data-ttu-id="92494-136">在请求正文中，提供 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92494-136">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92494-137">响应</span><span class="sxs-lookup"><span data-stu-id="92494-137">Response</span></span>

<span data-ttu-id="92494-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92494-138">If successful, this method returns `201 Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92494-139">示例</span><span class="sxs-lookup"><span data-stu-id="92494-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92494-140">请求</span><span class="sxs-lookup"><span data-stu-id="92494-140">Request</span></span>
<span data-ttu-id="92494-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92494-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="92494-142">响应</span><span class="sxs-lookup"><span data-stu-id="92494-142">Response</span></span>
<span data-ttu-id="92494-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92494-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
