---
title: 列出 mailFolder
description: 获取已登录的用户邮箱中的所有邮件文件夹。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8de6fa03cb0f7b6a85e2055d060101e598265b43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509929"
---
# <a name="list-mailfolders"></a><span data-ttu-id="bb810-103">列出 mailFolder</span><span class="sxs-lookup"><span data-stu-id="bb810-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb810-104">获取已登录的用户邮箱中的所有邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="bb810-104">Get all the mail folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb810-105">权限</span><span class="sxs-lookup"><span data-stu-id="bb810-105">Permissions</span></span>
<span data-ttu-id="bb810-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb810-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb810-108">Permission type</span></span>      | <span data-ttu-id="bb810-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb810-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb810-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb810-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb810-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb810-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bb810-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb810-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb810-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb810-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bb810-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb810-114">Application</span></span> | <span data-ttu-id="bb810-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb810-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb810-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb810-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb810-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb810-117">Optional query parameters</span></span>
<span data-ttu-id="bb810-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb810-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bb810-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb810-119">Request headers</span></span>
| <span data-ttu-id="bb810-120">标头</span><span class="sxs-lookup"><span data-stu-id="bb810-120">Header</span></span>       | <span data-ttu-id="bb810-121">值</span><span class="sxs-lookup"><span data-stu-id="bb810-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb810-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb810-122">Authorization</span></span>  | <span data-ttu-id="bb810-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb810-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb810-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb810-125">Content-Type</span></span>   | <span data-ttu-id="bb810-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb810-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb810-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb810-127">Request body</span></span>
<span data-ttu-id="bb810-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb810-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb810-129">响应</span><span class="sxs-lookup"><span data-stu-id="bb810-129">Response</span></span>

<span data-ttu-id="bb810-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb810-130">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb810-131">示例</span><span class="sxs-lookup"><span data-stu-id="bb810-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb810-132">请求</span><span class="sxs-lookup"><span data-stu-id="bb810-132">Request</span></span>
<span data-ttu-id="bb810-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb810-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="bb810-134">响应</span><span class="sxs-lookup"><span data-stu-id="bb810-134">Response</span></span>
<span data-ttu-id="bb810-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb810-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
