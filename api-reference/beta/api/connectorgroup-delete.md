---
title: 删除 connectorGroup
description: 删除 connectorGroup。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e8c7d0dc61338b10451f553421b74ad1b41f628f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943475"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="51a35-103">删除 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="51a35-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51a35-104">删除 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="51a35-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="51a35-105">权限</span><span class="sxs-lookup"><span data-stu-id="51a35-105">Permissions</span></span>
<span data-ttu-id="51a35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51a35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51a35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="51a35-108">Permission type</span></span>      | <span data-ttu-id="51a35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51a35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51a35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51a35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51a35-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51a35-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51a35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51a35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51a35-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="51a35-113">Not supported.</span></span>    |
|<span data-ttu-id="51a35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="51a35-114">Application</span></span> | <span data-ttu-id="51a35-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a35-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="51a35-116">**注意:** 连接器组不能有任何关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="51a35-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="51a35-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51a35-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="51a35-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="51a35-118">Request headers</span></span>
| <span data-ttu-id="51a35-119">名称</span><span class="sxs-lookup"><span data-stu-id="51a35-119">Name</span></span>       | <span data-ttu-id="51a35-120">说明</span><span class="sxs-lookup"><span data-stu-id="51a35-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51a35-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51a35-121">Authorization</span></span>  | <span data-ttu-id="51a35-122">负载.</span><span class="sxs-lookup"><span data-stu-id="51a35-122">Bearer.</span></span> <span data-ttu-id="51a35-123">必需</span><span class="sxs-lookup"><span data-stu-id="51a35-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="51a35-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="51a35-124">Request body</span></span>
<span data-ttu-id="51a35-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51a35-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51a35-126">响应</span><span class="sxs-lookup"><span data-stu-id="51a35-126">Response</span></span>

<span data-ttu-id="51a35-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="51a35-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51a35-129">示例</span><span class="sxs-lookup"><span data-stu-id="51a35-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51a35-130">请求</span><span class="sxs-lookup"><span data-stu-id="51a35-130">Request</span></span>
<span data-ttu-id="51a35-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51a35-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="51a35-132">响应</span><span class="sxs-lookup"><span data-stu-id="51a35-132">Response</span></span>
<span data-ttu-id="51a35-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51a35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
