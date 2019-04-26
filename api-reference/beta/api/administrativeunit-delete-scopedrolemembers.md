---
title: 删除 scopedRoleMember
description: 从管理单元中删除作用域角色成员。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 912575f5e9a63e6d7cce543681ff9efb6d8361b8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323011"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="27aba-103">删除 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="27aba-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27aba-104">从管理单元中删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="27aba-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="27aba-105">权限</span><span class="sxs-lookup"><span data-stu-id="27aba-105">Permissions</span></span>
<span data-ttu-id="27aba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27aba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27aba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="27aba-108">Permission type</span></span>      | <span data-ttu-id="27aba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27aba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27aba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27aba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27aba-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27aba-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27aba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27aba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27aba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="27aba-113">Not supported.</span></span>    |
|<span data-ttu-id="27aba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="27aba-114">Application</span></span> | <span data-ttu-id="27aba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27aba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27aba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27aba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="27aba-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="27aba-117">Request headers</span></span>
| <span data-ttu-id="27aba-118">名称</span><span class="sxs-lookup"><span data-stu-id="27aba-118">Name</span></span>       | <span data-ttu-id="27aba-119">说明</span><span class="sxs-lookup"><span data-stu-id="27aba-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27aba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="27aba-120">Authorization</span></span>  | <span data-ttu-id="27aba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27aba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27aba-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="27aba-123">Request body</span></span>
<span data-ttu-id="27aba-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27aba-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27aba-125">响应</span><span class="sxs-lookup"><span data-stu-id="27aba-125">Response</span></span>

<span data-ttu-id="27aba-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="27aba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27aba-128">示例</span><span class="sxs-lookup"><span data-stu-id="27aba-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27aba-129">请求</span><span class="sxs-lookup"><span data-stu-id="27aba-129">Request</span></span>
<span data-ttu-id="27aba-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27aba-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="27aba-131">响应</span><span class="sxs-lookup"><span data-stu-id="27aba-131">Response</span></span>
<span data-ttu-id="27aba-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27aba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
