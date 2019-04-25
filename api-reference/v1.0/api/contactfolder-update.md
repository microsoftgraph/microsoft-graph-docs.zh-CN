---
title: 更新 contactfolder
description: 更新 contactfolder 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 39a0869757fe42fd4502b194b84c3fe3e3edad68
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566106"
---
# <a name="update-contactfolder"></a><span data-ttu-id="3091c-103">更新 contactfolder</span><span class="sxs-lookup"><span data-stu-id="3091c-103">Update contactfolder</span></span>

<span data-ttu-id="3091c-104">更新 contactfolder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3091c-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3091c-105">权限</span><span class="sxs-lookup"><span data-stu-id="3091c-105">Permissions</span></span>
<span data-ttu-id="3091c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3091c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3091c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3091c-108">Permission type</span></span>      | <span data-ttu-id="3091c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3091c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3091c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3091c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3091c-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3091c-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3091c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3091c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3091c-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3091c-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3091c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3091c-114">Application</span></span> | <span data-ttu-id="3091c-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3091c-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3091c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3091c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3091c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3091c-117">Request headers</span></span>
| <span data-ttu-id="3091c-118">标头</span><span class="sxs-lookup"><span data-stu-id="3091c-118">Header</span></span>       | <span data-ttu-id="3091c-119">值</span><span class="sxs-lookup"><span data-stu-id="3091c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3091c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3091c-120">Authorization</span></span>  | <span data-ttu-id="3091c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3091c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3091c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3091c-123">Content-Type</span></span>  | <span data-ttu-id="3091c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3091c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3091c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3091c-126">Request body</span></span>
<span data-ttu-id="3091c-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3091c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3091c-130">属性</span><span class="sxs-lookup"><span data-stu-id="3091c-130">Property</span></span>     | <span data-ttu-id="3091c-131">类型</span><span class="sxs-lookup"><span data-stu-id="3091c-131">Type</span></span>   |<span data-ttu-id="3091c-132">说明</span><span class="sxs-lookup"><span data-stu-id="3091c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3091c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3091c-133">displayName</span></span>|<span data-ttu-id="3091c-134">String</span><span class="sxs-lookup"><span data-stu-id="3091c-134">String</span></span>|<span data-ttu-id="3091c-135">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3091c-135">The folder's display name.</span></span>|
|<span data-ttu-id="3091c-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="3091c-136">parentFolderId</span></span>|<span data-ttu-id="3091c-137">String</span><span class="sxs-lookup"><span data-stu-id="3091c-137">String</span></span>|<span data-ttu-id="3091c-138">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="3091c-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="3091c-139">响应</span><span class="sxs-lookup"><span data-stu-id="3091c-139">Response</span></span>

<span data-ttu-id="3091c-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3091c-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3091c-141">示例</span><span class="sxs-lookup"><span data-stu-id="3091c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3091c-142">请求</span><span class="sxs-lookup"><span data-stu-id="3091c-142">Request</span></span>
<span data-ttu-id="3091c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3091c-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="3091c-144">响应</span><span class="sxs-lookup"><span data-stu-id="3091c-144">Response</span></span>
<span data-ttu-id="3091c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3091c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
