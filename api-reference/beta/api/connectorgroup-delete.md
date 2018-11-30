---
title: 删除 connectorGroup
description: 删除 connectorGroup。
ms.openlocfilehash: 3ba4a5a06e25f2fb1568ab9d7d6e92104ea083de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042381"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="ba259-103">删除 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ba259-103">Delete connectorGroup</span></span>

> <span data-ttu-id="ba259-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba259-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba259-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba259-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba259-106">删除 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="ba259-106">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba259-107">权限</span><span class="sxs-lookup"><span data-stu-id="ba259-107">Permissions</span></span>
<span data-ttu-id="ba259-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba259-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ba259-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba259-110">Permission type</span></span>      | <span data-ttu-id="ba259-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba259-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba259-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba259-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba259-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba259-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba259-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba259-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba259-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba259-115">Not supported.</span></span>    |
|<span data-ttu-id="ba259-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba259-116">Application</span></span> | <span data-ttu-id="ba259-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba259-117">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ba259-118">**注意：** 连接器组不能有与之关联的任何连接器。</span><span class="sxs-lookup"><span data-stu-id="ba259-118">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="ba259-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba259-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ba259-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba259-120">Request headers</span></span>
| <span data-ttu-id="ba259-121">名称</span><span class="sxs-lookup"><span data-stu-id="ba259-121">Name</span></span>       | <span data-ttu-id="ba259-122">说明</span><span class="sxs-lookup"><span data-stu-id="ba259-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ba259-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba259-123">Authorization</span></span>  | <span data-ttu-id="ba259-124">持有者。</span><span class="sxs-lookup"><span data-stu-id="ba259-124">Bearer.</span></span> <span data-ttu-id="ba259-125">必需</span><span class="sxs-lookup"><span data-stu-id="ba259-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba259-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba259-126">Request body</span></span>
<span data-ttu-id="ba259-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba259-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba259-128">响应</span><span class="sxs-lookup"><span data-stu-id="ba259-128">Response</span></span>

<span data-ttu-id="ba259-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ba259-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba259-131">示例</span><span class="sxs-lookup"><span data-stu-id="ba259-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba259-132">请求</span><span class="sxs-lookup"><span data-stu-id="ba259-132">Request</span></span>
<span data-ttu-id="ba259-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba259-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="ba259-134">响应</span><span class="sxs-lookup"><span data-stu-id="ba259-134">Response</span></span>
<span data-ttu-id="ba259-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba259-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
