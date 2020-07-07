---
title: 删除 profileCardProperty
description: 删除 profileCardProperty 对象并删除配置文件卡片中的所有自定义项。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c2dd6ef082167f40c173386f18be7760118a966f
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051034"
---
# <a name="delete-profilecardproperty"></a><span data-ttu-id="8f357-103">删除 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="8f357-103">Delete profileCardProperty</span></span>

<span data-ttu-id="8f357-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f357-105">从组织的配置文件卡片中删除由其指定的[profileCardProperty](../resources/profilecardproperty.md)对象 `directoryPropertyName` ，并删除该属性的所有本地化的自定义项。</span><span class="sxs-lookup"><span data-stu-id="8f357-105">Delete the [profileCardProperty](../resources/profilecardproperty.md) object specified by its `directoryPropertyName` from the organization's profile card, and remove any localized customizations for that property.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f357-106">权限</span><span class="sxs-lookup"><span data-stu-id="8f357-106">Permissions</span></span>

<span data-ttu-id="8f357-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8f357-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8f357-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f357-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f357-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f357-109">Permission type</span></span>                        | <span data-ttu-id="8f357-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f357-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f357-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f357-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f357-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="8f357-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8f357-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f357-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f357-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f357-114">Not supported.</span></span>                              |
| <span data-ttu-id="8f357-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f357-115">Application</span></span>                            | <span data-ttu-id="8f357-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f357-116">Not supported.</span></span>                              |

><span data-ttu-id="8f357-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="8f357-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="8f357-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f357-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a><span data-ttu-id="8f357-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f357-119">Request headers</span></span>

| <span data-ttu-id="8f357-120">名称</span><span class="sxs-lookup"><span data-stu-id="8f357-120">Name</span></span>          | <span data-ttu-id="8f357-121">说明</span><span class="sxs-lookup"><span data-stu-id="8f357-121">Description</span></span>    |
|:--------------|:---------------|
| <span data-ttu-id="8f357-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f357-122">Authorization</span></span> | <span data-ttu-id="8f357-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8f357-123">Bearer {token}.</span></span> <span data-ttu-id="8f357-124">Required.</span><span class="sxs-lookup"><span data-stu-id="8f357-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f357-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f357-125">Request body</span></span>

<span data-ttu-id="8f357-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f357-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f357-127">响应</span><span class="sxs-lookup"><span data-stu-id="8f357-127">Response</span></span>

<span data-ttu-id="8f357-128">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="8f357-128">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="8f357-129">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="8f357-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f357-130">示例</span><span class="sxs-lookup"><span data-stu-id="8f357-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f357-131">请求</span><span class="sxs-lookup"><span data-stu-id="8f357-131">Request</span></span>

<span data-ttu-id="8f357-132">下面的示例演示如何从组织的配置文件卡片中删除名为 "Fax" 的属性。</span><span class="sxs-lookup"><span data-stu-id="8f357-132">The following example shows how to delete the attribute named "Fax" from the profile card for the organization.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/fax
```

### <a name="response"></a><span data-ttu-id="8f357-133">响应</span><span class="sxs-lookup"><span data-stu-id="8f357-133">Response</span></span>

<span data-ttu-id="8f357-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f357-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
