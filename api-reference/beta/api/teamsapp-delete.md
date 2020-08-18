---
title: 删除 teamsApp
description: " (租户应用程序目录) 中删除组织的应用程序目录中的团队应用程序。 "
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 432af0167562d34ca006b05901ad5fcb7529a51c
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790495"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="391f4-103">删除 teamsApp</span><span class="sxs-lookup"><span data-stu-id="391f4-103">Delete teamsApp</span></span>

<span data-ttu-id="391f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="391f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="391f4-105"> (租户应用程序目录) 中删除组织的应用程序目录中的 [应用](../resources/teamsapp.md) 程序。</span><span class="sxs-lookup"><span data-stu-id="391f4-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="391f4-106">若要删除应用程序，必须将应用程序的 **distributionMethod** 属性设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="391f4-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="391f4-107">您还可以使用此 API 从审阅过程中删除已提交的应用程序。</span><span class="sxs-lookup"><span data-stu-id="391f4-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="391f4-108">权限</span><span class="sxs-lookup"><span data-stu-id="391f4-108">Permissions</span></span>

<span data-ttu-id="391f4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="391f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="391f4-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="391f4-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="391f4-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="391f4-112">Permission Type</span></span>                        | <span data-ttu-id="391f4-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="391f4-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="391f4-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="391f4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="391f4-115">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="391f4-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="391f4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="391f4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="391f4-117">AppCatalog</span><span class="sxs-lookup"><span data-stu-id="391f4-117">AppCatalog.Submit</span></span> |
| <span data-ttu-id="391f4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="391f4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="391f4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="391f4-119">Not supported.</span></span>|
| <span data-ttu-id="391f4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="391f4-120">Application</span></span>                            | <span data-ttu-id="391f4-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="391f4-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="391f4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="391f4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="391f4-123">从应用程序目录中删除应用程序：</span><span class="sxs-lookup"><span data-stu-id="391f4-123">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="391f4-124">若要删除已提交但尚未批准的应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="391f4-124">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="391f4-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="391f4-125">Request headers</span></span>

| <span data-ttu-id="391f4-126">标头</span><span class="sxs-lookup"><span data-stu-id="391f4-126">Header</span></span>        | <span data-ttu-id="391f4-127">值</span><span class="sxs-lookup"><span data-stu-id="391f4-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="391f4-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="391f4-128">Authorization</span></span> | <span data-ttu-id="391f4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="391f4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="391f4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="391f4-131">Request body</span></span>

<span data-ttu-id="391f4-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="391f4-132">Do not supply a request body for this method.</span></span>

><span data-ttu-id="391f4-133">**注意：** 使用从 [列表已发布的应用程序](./teamsapp-list.md) 调用返回的 ID 引用要删除的应用程序。</span><span class="sxs-lookup"><span data-stu-id="391f4-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="391f4-134">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="391f4-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="391f4-135">响应</span><span class="sxs-lookup"><span data-stu-id="391f4-135">Response</span></span>

<span data-ttu-id="391f4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="391f4-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="391f4-138">示例</span><span class="sxs-lookup"><span data-stu-id="391f4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="391f4-139">请求</span><span class="sxs-lookup"><span data-stu-id="391f4-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="391f4-140">响应</span><span class="sxs-lookup"><span data-stu-id="391f4-140">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
