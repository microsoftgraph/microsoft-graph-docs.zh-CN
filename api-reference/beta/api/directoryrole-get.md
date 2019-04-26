---
title: 获取 DirectoryRole
description: 检索 directoryRole 对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bdb63bfacf28f4851109fcdbc1cd0538cafb0024
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325811"
---
# <a name="get-directoryrole"></a><span data-ttu-id="c5fdf-103">获取 DirectoryRole</span><span class="sxs-lookup"><span data-stu-id="c5fdf-103">Get directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5fdf-104">检索 directoryRole 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-104">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5fdf-105">权限</span><span class="sxs-lookup"><span data-stu-id="c5fdf-105">Permissions</span></span>
<span data-ttu-id="c5fdf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5fdf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5fdf-108">Permission type</span></span>      | <span data-ttu-id="c5fdf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5fdf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5fdf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fdf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fdf-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5fdf-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5fdf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fdf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fdf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-113">Not supported.</span></span>    |
|<span data-ttu-id="c5fdf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5fdf-114">Application</span></span> | <span data-ttu-id="c5fdf-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fdf-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5fdf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5fdf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5fdf-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5fdf-117">Optional query parameters</span></span>
<span data-ttu-id="c5fdf-118">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5fdf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5fdf-119">Request headers</span></span>
| <span data-ttu-id="c5fdf-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5fdf-120">Name</span></span>       | <span data-ttu-id="c5fdf-121">类型</span><span class="sxs-lookup"><span data-stu-id="c5fdf-121">Type</span></span> | <span data-ttu-id="c5fdf-122">说明</span><span class="sxs-lookup"><span data-stu-id="c5fdf-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5fdf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fdf-123">Authorization</span></span>  | <span data-ttu-id="c5fdf-124">string</span><span class="sxs-lookup"><span data-stu-id="c5fdf-124">string</span></span>  | <span data-ttu-id="c5fdf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5fdf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5fdf-127">Request body</span></span>
<span data-ttu-id="c5fdf-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5fdf-129">响应</span><span class="sxs-lookup"><span data-stu-id="c5fdf-129">Response</span></span>

<span data-ttu-id="c5fdf-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5fdf-131">示例</span><span class="sxs-lookup"><span data-stu-id="c5fdf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5fdf-132">请求</span><span class="sxs-lookup"><span data-stu-id="c5fdf-132">Request</span></span>
<span data-ttu-id="c5fdf-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="c5fdf-134">响应</span><span class="sxs-lookup"><span data-stu-id="c5fdf-134">Response</span></span>
<span data-ttu-id="c5fdf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5fdf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
