---
title: 删除 connectorGroup
description: 删除 connectorGroup。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 960fe8a61dc00eaddcd6c96e255ea7cb7033434c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437481"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="f6a0b-103">删除 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f6a0b-103">Delete connectorGroup</span></span>

<span data-ttu-id="f6a0b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6a0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6a0b-105">删除 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-105">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6a0b-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6a0b-106">Permissions</span></span>
<span data-ttu-id="f6a0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6a0b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6a0b-109">Permission type</span></span>      | <span data-ttu-id="f6a0b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6a0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6a0b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6a0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6a0b-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6a0b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6a0b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6a0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6a0b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-114">Not supported.</span></span>    |
|<span data-ttu-id="f6a0b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6a0b-115">Application</span></span> | <span data-ttu-id="f6a0b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6a0b-116">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f6a0b-117">**注意：** 连接器组不能有任何关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-117">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="f6a0b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6a0b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f6a0b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6a0b-119">Request headers</span></span>
| <span data-ttu-id="f6a0b-120">名称</span><span class="sxs-lookup"><span data-stu-id="f6a0b-120">Name</span></span>       | <span data-ttu-id="f6a0b-121">说明</span><span class="sxs-lookup"><span data-stu-id="f6a0b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f6a0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6a0b-122">Authorization</span></span>  | <span data-ttu-id="f6a0b-123">负载.</span><span class="sxs-lookup"><span data-stu-id="f6a0b-123">Bearer.</span></span> <span data-ttu-id="f6a0b-124">必需</span><span class="sxs-lookup"><span data-stu-id="f6a0b-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6a0b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6a0b-125">Request body</span></span>
<span data-ttu-id="f6a0b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6a0b-127">响应</span><span class="sxs-lookup"><span data-stu-id="f6a0b-127">Response</span></span>

<span data-ttu-id="f6a0b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6a0b-130">示例</span><span class="sxs-lookup"><span data-stu-id="f6a0b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6a0b-131">请求</span><span class="sxs-lookup"><span data-stu-id="f6a0b-131">Request</span></span>
<span data-ttu-id="f6a0b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="f6a0b-133">响应</span><span class="sxs-lookup"><span data-stu-id="f6a0b-133">Response</span></span>
<span data-ttu-id="f6a0b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6a0b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
