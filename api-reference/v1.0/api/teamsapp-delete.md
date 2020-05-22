---
title: 权限
description: '从组织的应用程序目录中删除应用程序（租户应用程序目录）。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8fe918b6e584fb3f22e00c2ca488cb7ef2937bdd
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345889"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="9785e-103">从组织的应用程序目录中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="9785e-103">Remove an app from your organization's app catalog</span></span>

<span data-ttu-id="9785e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9785e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="9785e-105">从组织的应用程序目录中删除[应用程序](../resources/teamsapp.md)（租户应用程序目录）。</span><span class="sxs-lookup"><span data-stu-id="9785e-105">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="9785e-106">若要从组织的应用程序目录中删除应用程序，请 `organization` 在[teamsCatalogApp](../resources/teamsapp.md)资源中将其指定为**distributionMethod** 。</span><span class="sxs-lookup"><span data-stu-id="9785e-106">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="9785e-107">权限</span><span class="sxs-lookup"><span data-stu-id="9785e-107">Permissions</span></span>

<span data-ttu-id="9785e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="9785e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="9785e-110">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9785e-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="9785e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9785e-111">Permission Type</span></span>                        | <span data-ttu-id="9785e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9785e-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="9785e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9785e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9785e-114">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="9785e-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="9785e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9785e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9785e-116">不支持</span><span class="sxs-lookup"><span data-stu-id="9785e-116">Not supported</span></span>|
| <span data-ttu-id="9785e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9785e-117">Application</span></span>                            | <span data-ttu-id="9785e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9785e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9785e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9785e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9785e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9785e-120">Request headers</span></span>

| <span data-ttu-id="9785e-121">标头</span><span class="sxs-lookup"><span data-stu-id="9785e-121">Header</span></span>        | <span data-ttu-id="9785e-122">值</span><span class="sxs-lookup"><span data-stu-id="9785e-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="9785e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9785e-123">Authorization</span></span> | <span data-ttu-id="9785e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9785e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9785e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9785e-126">Request body</span></span>

<span data-ttu-id="9785e-127">无。</span><span class="sxs-lookup"><span data-stu-id="9785e-127">None.</span></span>

><span data-ttu-id="9785e-128">**注意：** 使用从[列表已发布的应用程序](./teamsapp-list.md)调用中返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9785e-128">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="9785e-129">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="9785e-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="9785e-130">响应</span><span class="sxs-lookup"><span data-stu-id="9785e-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="9785e-131">示例</span><span class="sxs-lookup"><span data-stu-id="9785e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9785e-132">请求</span><span class="sxs-lookup"><span data-stu-id="9785e-132">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="9785e-133">响应</span><span class="sxs-lookup"><span data-stu-id="9785e-133">Response</span></span>

```http
HTTP/1.1 204 No Content
```
