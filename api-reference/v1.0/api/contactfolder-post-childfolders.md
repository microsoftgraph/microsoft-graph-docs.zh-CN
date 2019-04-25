---
title: 创建 ContactFolder
description: '创建新的 contactFolder 作为指定文件夹的子文件夹。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f7cd5d35bce0e23fcc10f88dde524d3e80faebf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566197"
---
# <a name="create-contactfolder"></a><span data-ttu-id="dd916-103">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="dd916-103">Create ContactFolder</span></span>

<span data-ttu-id="dd916-104">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="dd916-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="dd916-105">还可以[在用户的默认联系人文件夹下创建新的 contactFolder](user-post-contactfolders.md)。</span><span class="sxs-lookup"><span data-stu-id="dd916-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="dd916-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd916-106">Permissions</span></span>
<span data-ttu-id="dd916-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd916-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd916-109">Permission type</span></span>      | <span data-ttu-id="dd916-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd916-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd916-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd916-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd916-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd916-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dd916-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd916-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd916-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd916-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="dd916-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd916-115">Application</span></span> | <span data-ttu-id="dd916-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd916-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd916-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd916-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="dd916-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd916-118">Request headers</span></span>
| <span data-ttu-id="dd916-119">标头</span><span class="sxs-lookup"><span data-stu-id="dd916-119">Header</span></span>       | <span data-ttu-id="dd916-120">值</span><span class="sxs-lookup"><span data-stu-id="dd916-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dd916-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd916-121">Authorization</span></span>  | <span data-ttu-id="dd916-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd916-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dd916-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd916-124">Content-Type</span></span>  | <span data-ttu-id="dd916-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="dd916-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd916-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd916-127">Request body</span></span>
<span data-ttu-id="dd916-128">在请求正文中，提供 [ContactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd916-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dd916-129">响应</span><span class="sxs-lookup"><span data-stu-id="dd916-129">Response</span></span>

<span data-ttu-id="dd916-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd916-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd916-131">示例</span><span class="sxs-lookup"><span data-stu-id="dd916-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd916-132">请求</span><span class="sxs-lookup"><span data-stu-id="dd916-132">Request</span></span>
<span data-ttu-id="dd916-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd916-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="dd916-134">在请求正文中，提供 [contactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd916-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dd916-135">响应</span><span class="sxs-lookup"><span data-stu-id="dd916-135">Response</span></span>
<span data-ttu-id="dd916-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd916-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
