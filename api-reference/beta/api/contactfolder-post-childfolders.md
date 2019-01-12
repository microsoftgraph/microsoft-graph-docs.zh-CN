---
title: 创建 ContactFolder
description: '创建新的 contactFolder 作为指定文件夹的子文件夹。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 66061d86b3c3894c165788cd408b22b8824b34f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991767"
---
# <a name="create-contactfolder"></a><span data-ttu-id="a4024-103">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="a4024-103">Create ContactFolder</span></span>

> <span data-ttu-id="a4024-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4024-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4024-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4024-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4024-106">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="a4024-106">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="a4024-107">还可以[在用户的默认联系人文件夹下创建新的 contactFolder](user-post-contactfolders.md)。</span><span class="sxs-lookup"><span data-stu-id="a4024-107">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a4024-108">权限</span><span class="sxs-lookup"><span data-stu-id="a4024-108">Permissions</span></span>
<span data-ttu-id="a4024-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4024-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4024-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4024-111">Permission type</span></span>      | <span data-ttu-id="a4024-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4024-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4024-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4024-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a4024-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4024-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a4024-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4024-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4024-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4024-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a4024-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4024-117">Application</span></span> | <span data-ttu-id="a4024-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4024-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4024-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4024-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="a4024-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4024-120">Request headers</span></span>
| <span data-ttu-id="a4024-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4024-121">Header</span></span>       | <span data-ttu-id="a4024-122">值</span><span class="sxs-lookup"><span data-stu-id="a4024-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4024-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4024-123">Authorization</span></span>  | <span data-ttu-id="a4024-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4024-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4024-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4024-126">Content-Type</span></span>  | <span data-ttu-id="a4024-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a4024-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4024-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4024-129">Request body</span></span>
<span data-ttu-id="a4024-130">在请求正文中，提供 [ContactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4024-130">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a4024-131">响应</span><span class="sxs-lookup"><span data-stu-id="a4024-131">Response</span></span>

<span data-ttu-id="a4024-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4024-132">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4024-133">示例</span><span class="sxs-lookup"><span data-stu-id="a4024-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4024-134">请求</span><span class="sxs-lookup"><span data-stu-id="a4024-134">Request</span></span>
<span data-ttu-id="a4024-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4024-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="a4024-136">在请求正文中，提供 [contactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4024-136">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a4024-137">响应</span><span class="sxs-lookup"><span data-stu-id="a4024-137">Response</span></span>
<span data-ttu-id="a4024-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4024-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
