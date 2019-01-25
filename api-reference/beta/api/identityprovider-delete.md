---
title: 删除 identityProvider
description: 删除现有 identityProvider。
localization_priority: Normal
ms.openlocfilehash: bb64f10b656697ab2cf611dd9be0468c295b15e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514353"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="1f94c-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="1f94c-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f94c-104">删除现有[identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="1f94c-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f94c-105">权限</span><span class="sxs-lookup"><span data-stu-id="1f94c-105">Permissions</span></span>

<span data-ttu-id="1f94c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f94c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f94c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f94c-108">Permission type</span></span>      | <span data-ttu-id="1f94c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f94c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f94c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f94c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1f94c-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f94c-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1f94c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f94c-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1f94c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f94c-113">Not supported.</span></span>|
|<span data-ttu-id="1f94c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f94c-114">Application</span></span>|<span data-ttu-id="1f94c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f94c-115">Not supported.</span></span>|

<span data-ttu-id="1f94c-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="1f94c-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="1f94c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f94c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1f94c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f94c-118">Request headers</span></span>

|<span data-ttu-id="1f94c-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f94c-119">Name</span></span>|<span data-ttu-id="1f94c-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f94c-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1f94c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f94c-121">Authorization</span></span>|<span data-ttu-id="1f94c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f94c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f94c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f94c-124">Request body</span></span>

<span data-ttu-id="1f94c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f94c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f94c-126">响应</span><span class="sxs-lookup"><span data-stu-id="1f94c-126">Response</span></span>

<span data-ttu-id="1f94c-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1f94c-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f94c-128">示例</span><span class="sxs-lookup"><span data-stu-id="1f94c-128">Example</span></span>

<span data-ttu-id="1f94c-129">下面的示例删除**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="1f94c-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="1f94c-130">请求</span><span class="sxs-lookup"><span data-stu-id="1f94c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="1f94c-131">响应</span><span class="sxs-lookup"><span data-stu-id="1f94c-131">Response</span></span>

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
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
