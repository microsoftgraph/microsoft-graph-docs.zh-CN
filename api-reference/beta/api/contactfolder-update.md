---
title: 更新 contactfolder
description: 更新 contactfolder 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9b2244f17bf877c1f52ae5de812f65ba1eae3b98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956148"
---
# <a name="update-contactfolder"></a><span data-ttu-id="f937e-103">更新 contactfolder</span><span class="sxs-lookup"><span data-stu-id="f937e-103">Update contactfolder</span></span>

> <span data-ttu-id="f937e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f937e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f937e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f937e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f937e-106">更新 contactfolder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f937e-106">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f937e-107">权限</span><span class="sxs-lookup"><span data-stu-id="f937e-107">Permissions</span></span>
<span data-ttu-id="f937e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f937e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f937e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f937e-110">Permission type</span></span>      | <span data-ttu-id="f937e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f937e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f937e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f937e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f937e-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f937e-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f937e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f937e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f937e-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f937e-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f937e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f937e-116">Application</span></span> | <span data-ttu-id="f937e-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f937e-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f937e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f937e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f937e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f937e-119">Request headers</span></span>
| <span data-ttu-id="f937e-120">标头</span><span class="sxs-lookup"><span data-stu-id="f937e-120">Header</span></span>       | <span data-ttu-id="f937e-121">值</span><span class="sxs-lookup"><span data-stu-id="f937e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f937e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f937e-122">Authorization</span></span>  | <span data-ttu-id="f937e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f937e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f937e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f937e-125">Content-Type</span></span>  | <span data-ttu-id="f937e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f937e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f937e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f937e-128">Request body</span></span>
<span data-ttu-id="f937e-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f937e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f937e-132">属性</span><span class="sxs-lookup"><span data-stu-id="f937e-132">Property</span></span>     | <span data-ttu-id="f937e-133">类型</span><span class="sxs-lookup"><span data-stu-id="f937e-133">Type</span></span>   |<span data-ttu-id="f937e-134">说明</span><span class="sxs-lookup"><span data-stu-id="f937e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f937e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f937e-135">displayName</span></span>|<span data-ttu-id="f937e-136">String</span><span class="sxs-lookup"><span data-stu-id="f937e-136">String</span></span>|<span data-ttu-id="f937e-137">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f937e-137">The folder's display name.</span></span>|
|<span data-ttu-id="f937e-138">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="f937e-138">parentFolderId</span></span>|<span data-ttu-id="f937e-139">String</span><span class="sxs-lookup"><span data-stu-id="f937e-139">String</span></span>|<span data-ttu-id="f937e-140">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="f937e-140">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="f937e-141">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="f937e-141">wellKnownName</span></span>|<span data-ttu-id="f937e-142">string</span><span class="sxs-lookup"><span data-stu-id="f937e-142">string</span></span>|<span data-ttu-id="f937e-143">如果文件夹为识别的文件夹的文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="f937e-143">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="f937e-144">当前`contacts`是仅识别联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="f937e-144">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="f937e-145">响应</span><span class="sxs-lookup"><span data-stu-id="f937e-145">Response</span></span>

<span data-ttu-id="f937e-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [contactFolder](../resources/contactfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f937e-146">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f937e-147">示例</span><span class="sxs-lookup"><span data-stu-id="f937e-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f937e-148">请求</span><span class="sxs-lookup"><span data-stu-id="f937e-148">Request</span></span>
<span data-ttu-id="f937e-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f937e-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="f937e-150">响应</span><span class="sxs-lookup"><span data-stu-id="f937e-150">Response</span></span>
<span data-ttu-id="f937e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f937e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "wellKnownName": "wellKnownName-value",
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
