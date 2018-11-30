---
title: 创建 Outlook 类别
description: 在用户主类别列表中创建 outlookCategory 对象。
ms.openlocfilehash: a3b948b7996a54676e98d348b5777e831c92d298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041701"
---
# <a name="create-outlook-category"></a><span data-ttu-id="1035a-103">创建 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="1035a-103">Create Outlook category</span></span>

> <span data-ttu-id="1035a-104">**重要说明**： 在 Microsoft Graph 中的 /beta 版本下的 Api 在预览，并会受到更改。</span><span class="sxs-lookup"><span data-stu-id="1035a-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1035a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1035a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1035a-106">在用户主类别列表中创建 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1035a-106">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="1035a-107">权限</span><span class="sxs-lookup"><span data-stu-id="1035a-107">Permissions</span></span>
<span data-ttu-id="1035a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1035a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1035a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1035a-110">Permission type</span></span>      | <span data-ttu-id="1035a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1035a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1035a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1035a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1035a-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1035a-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1035a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1035a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1035a-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1035a-115">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="1035a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1035a-116">Application</span></span> | <span data-ttu-id="1035a-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1035a-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1035a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1035a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="1035a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1035a-119">Request headers</span></span>
| <span data-ttu-id="1035a-120">名称</span><span class="sxs-lookup"><span data-stu-id="1035a-120">Name</span></span>       | <span data-ttu-id="1035a-121">说明</span><span class="sxs-lookup"><span data-stu-id="1035a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1035a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1035a-122">Authorization</span></span>  | <span data-ttu-id="1035a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1035a-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1035a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1035a-125">Request body</span></span>
<span data-ttu-id="1035a-126">在请求正文中，提供 [outlookCategory](../resources/outlookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1035a-126">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1035a-127">响应</span><span class="sxs-lookup"><span data-stu-id="1035a-127">Response</span></span>

<span data-ttu-id="1035a-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1035a-128">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1035a-129">示例</span><span class="sxs-lookup"><span data-stu-id="1035a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1035a-130">请求</span><span class="sxs-lookup"><span data-stu-id="1035a-130">Request</span></span>
<span data-ttu-id="1035a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1035a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="1035a-132">在请求正文中，提供 [outlookCategory](../resources/outlookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1035a-132">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1035a-133">响应</span><span class="sxs-lookup"><span data-stu-id="1035a-133">Response</span></span>
<span data-ttu-id="1035a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1035a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->