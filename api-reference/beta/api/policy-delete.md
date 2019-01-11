---
title: 删除策略
description: 删除策略。
localization_priority: Normal
ms.openlocfilehash: 66772865fdff5ebf4b111cae91e60b00707bf6a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875360"
---
# <a name="delete-policy"></a><span data-ttu-id="a5cf9-103">删除策略</span><span class="sxs-lookup"><span data-stu-id="a5cf9-103">Delete Policy</span></span>

> <span data-ttu-id="a5cf9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5cf9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5cf9-106">删除[策略](../resources/policy.md)。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-106">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5cf9-107">权限</span><span class="sxs-lookup"><span data-stu-id="a5cf9-107">Permissions</span></span>
<span data-ttu-id="a5cf9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5cf9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5cf9-110">Permission type</span></span>      | <span data-ttu-id="a5cf9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5cf9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5cf9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5cf9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5cf9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5cf9-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5cf9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5cf9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5cf9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-115">Not supported.</span></span>    |
|<span data-ttu-id="a5cf9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5cf9-116">Application</span></span> | <span data-ttu-id="a5cf9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5cf9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5cf9-118">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a5cf9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5cf9-119">Request headers</span></span>
| <span data-ttu-id="a5cf9-120">名称</span><span class="sxs-lookup"><span data-stu-id="a5cf9-120">Name</span></span>       | <span data-ttu-id="a5cf9-121">类型</span><span class="sxs-lookup"><span data-stu-id="a5cf9-121">Type</span></span> | <span data-ttu-id="a5cf9-122">说明</span><span class="sxs-lookup"><span data-stu-id="a5cf9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5cf9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5cf9-123">Authorization</span></span>  | <span data-ttu-id="a5cf9-124">string</span><span class="sxs-lookup"><span data-stu-id="a5cf9-124">string</span></span>  | <span data-ttu-id="a5cf9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5cf9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5cf9-127">Request body</span></span>
<span data-ttu-id="a5cf9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5cf9-129">响应</span><span class="sxs-lookup"><span data-stu-id="a5cf9-129">Response</span></span>

<span data-ttu-id="a5cf9-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="a5cf9-131">如果不成功...</span><span class="sxs-lookup"><span data-stu-id="a5cf9-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="a5cf9-132">示例</span><span class="sxs-lookup"><span data-stu-id="a5cf9-132">Example</span></span>
<span data-ttu-id="a5cf9-133">下面的示例删除策略。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-133">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="a5cf9-134">请求</span><span class="sxs-lookup"><span data-stu-id="a5cf9-134">Request</span></span>
<span data-ttu-id="a5cf9-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-135">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="a5cf9-136">响应</span><span class="sxs-lookup"><span data-stu-id="a5cf9-136">Response</span></span>
<span data-ttu-id="a5cf9-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5cf9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
