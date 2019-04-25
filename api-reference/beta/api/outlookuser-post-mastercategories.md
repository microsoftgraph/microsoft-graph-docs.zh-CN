---
title: 创建 Outlook 类别
description: 在用户主类别列表中创建 outlookCategory 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b9cf9ed2ca82e2f676ae1241f64ce361e0004437
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539621"
---
# <a name="create-outlook-category"></a><span data-ttu-id="530a6-103">创建 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="530a6-103">Create Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="530a6-104">在用户主类别列表中创建 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="530a6-104">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="530a6-105">权限</span><span class="sxs-lookup"><span data-stu-id="530a6-105">Permissions</span></span>
<span data-ttu-id="530a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="530a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="530a6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="530a6-108">Permission type</span></span>      | <span data-ttu-id="530a6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="530a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="530a6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="530a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="530a6-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="530a6-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="530a6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="530a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="530a6-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="530a6-113">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="530a6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="530a6-114">Application</span></span> | <span data-ttu-id="530a6-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="530a6-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="530a6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="530a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="530a6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="530a6-117">Request headers</span></span>
| <span data-ttu-id="530a6-118">名称</span><span class="sxs-lookup"><span data-stu-id="530a6-118">Name</span></span>       | <span data-ttu-id="530a6-119">说明</span><span class="sxs-lookup"><span data-stu-id="530a6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="530a6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="530a6-120">Authorization</span></span>  | <span data-ttu-id="530a6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="530a6-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="530a6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="530a6-123">Request body</span></span>
<span data-ttu-id="530a6-124">在请求正文中，提供 [outlookCategory](../resources/outlookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="530a6-124">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="530a6-125">响应</span><span class="sxs-lookup"><span data-stu-id="530a6-125">Response</span></span>

<span data-ttu-id="530a6-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="530a6-126">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="530a6-127">示例</span><span class="sxs-lookup"><span data-stu-id="530a6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="530a6-128">请求</span><span class="sxs-lookup"><span data-stu-id="530a6-128">Request</span></span>
<span data-ttu-id="530a6-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="530a6-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="530a6-130">在请求正文中，提供 [outlookCategory](../resources/outlookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="530a6-130">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="530a6-131">响应</span><span class="sxs-lookup"><span data-stu-id="530a6-131">Response</span></span>
<span data-ttu-id="530a6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="530a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "".
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-mastercategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
