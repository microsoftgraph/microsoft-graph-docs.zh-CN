---
title: 删除成员
description: 使用此 API 可删除成员 （用户或组） 从一个管理单元。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 09cb727c60e102786948311f10df48f9230a9dd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865196"
---
# <a name="remove-a-member"></a><span data-ttu-id="71a67-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="71a67-103">Remove a member</span></span>

> <span data-ttu-id="71a67-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="71a67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71a67-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="71a67-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71a67-106">使用此 API 可删除成员 （用户或组） 从一个管理单元。</span><span class="sxs-lookup"><span data-stu-id="71a67-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="71a67-107">权限</span><span class="sxs-lookup"><span data-stu-id="71a67-107">Permissions</span></span>
<span data-ttu-id="71a67-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71a67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="71a67-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71a67-110">Permission type</span></span>      | <span data-ttu-id="71a67-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71a67-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71a67-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71a67-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71a67-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71a67-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71a67-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71a67-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71a67-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71a67-115">Not supported.</span></span>    |
|<span data-ttu-id="71a67-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71a67-116">Application</span></span> | <span data-ttu-id="71a67-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71a67-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71a67-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71a67-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="71a67-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71a67-119">Request headers</span></span>
| <span data-ttu-id="71a67-120">名称</span><span class="sxs-lookup"><span data-stu-id="71a67-120">Name</span></span>      |<span data-ttu-id="71a67-121">说明</span><span class="sxs-lookup"><span data-stu-id="71a67-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71a67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71a67-122">Authorization</span></span>  | <span data-ttu-id="71a67-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71a67-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71a67-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="71a67-125">Request body</span></span>
<span data-ttu-id="71a67-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71a67-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71a67-127">响应</span><span class="sxs-lookup"><span data-stu-id="71a67-127">Response</span></span>

<span data-ttu-id="71a67-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71a67-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71a67-130">示例</span><span class="sxs-lookup"><span data-stu-id="71a67-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71a67-131">请求</span><span class="sxs-lookup"><span data-stu-id="71a67-131">Request</span></span>
<span data-ttu-id="71a67-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71a67-132">Here is an example of the request.</span></span> <span data-ttu-id="71a67-133">在下面的示例中，id1 的目标管理单元，表示的标识符和 id2 表示要从指定的管理单元中删除的成员用户或组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="71a67-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="71a67-134">响应</span><span class="sxs-lookup"><span data-stu-id="71a67-134">Response</span></span>
<span data-ttu-id="71a67-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71a67-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
