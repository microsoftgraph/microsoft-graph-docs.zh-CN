---
title: 创建 ContactFolder
description: 在用户的默认联系人文件夹下创建新的 contactFolder。
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76f7f7592657e913322343426c07575344fc4d68
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473547"
---
# <a name="create-contactfolder"></a><span data-ttu-id="25e27-103">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="25e27-103">Create ContactFolder</span></span>

<span data-ttu-id="25e27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e27-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25e27-105">在用户的默认联系人文件夹下创建新的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="25e27-105">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="25e27-106">还可以[创建新的 contactfolder，作为任意指定联系人文件夹的子文件夹](contactfolder-post-childfolders.md)。</span><span class="sxs-lookup"><span data-stu-id="25e27-106">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="25e27-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="25e27-107">Permissions</span></span>
<span data-ttu-id="25e27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25e27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e27-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25e27-110">Permission type</span></span>      | <span data-ttu-id="25e27-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25e27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e27-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25e27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25e27-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25e27-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="25e27-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25e27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25e27-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25e27-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="25e27-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25e27-116">Application</span></span> | <span data-ttu-id="25e27-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25e27-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="25e27-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25e27-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="25e27-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25e27-119">Request headers</span></span>
| <span data-ttu-id="25e27-120">标头</span><span class="sxs-lookup"><span data-stu-id="25e27-120">Header</span></span>       | <span data-ttu-id="25e27-121">值</span><span class="sxs-lookup"><span data-stu-id="25e27-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25e27-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25e27-122">Authorization</span></span>  | <span data-ttu-id="25e27-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25e27-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="25e27-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25e27-125">Content-Type</span></span>  | <span data-ttu-id="25e27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25e27-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25e27-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="25e27-127">Request body</span></span>
<span data-ttu-id="25e27-128">在请求正文中，提供 [ContactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25e27-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="25e27-129">响应</span><span class="sxs-lookup"><span data-stu-id="25e27-129">Response</span></span>

<span data-ttu-id="25e27-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ContactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25e27-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25e27-131">示例</span><span class="sxs-lookup"><span data-stu-id="25e27-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="25e27-132">请求</span><span class="sxs-lookup"><span data-stu-id="25e27-132">Request</span></span>
<span data-ttu-id="25e27-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25e27-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts"
}
```

<span data-ttu-id="25e27-134">在请求正文中，提供 [contactFolder](../resources/contactfolder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25e27-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="25e27-135">响应</span><span class="sxs-lookup"><span data-stu-id="25e27-135">Response</span></span>
<span data-ttu-id="25e27-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25e27-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "parentFolderId": "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==",
  "displayName": "Important contacts",
  "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy04MDU0LTBkOTFkY2Y5NzE1NAAuAAAAAADESc12GiymT5Zp9IHtHnWZAQA2t6otiDF0TYOkcEEh3vhfAAAGgUC1AAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

