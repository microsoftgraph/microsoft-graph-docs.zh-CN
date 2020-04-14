---
title: 删除策略
description: 删除策略。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: c24a20133d79e32d0a2e5559fbc2309b5863aa9b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450884"
---
# <a name="delete-policy"></a><span data-ttu-id="b7aab-103">删除策略</span><span class="sxs-lookup"><span data-stu-id="b7aab-103">Delete Policy</span></span>

<span data-ttu-id="b7aab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7aab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7aab-105">删除[策略](../resources/policy.md)。</span><span class="sxs-lookup"><span data-stu-id="b7aab-105">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7aab-106">权限</span><span class="sxs-lookup"><span data-stu-id="b7aab-106">Permissions</span></span>
<span data-ttu-id="b7aab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7aab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7aab-109">Permission type</span></span>      | <span data-ttu-id="b7aab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7aab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7aab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7aab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7aab-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7aab-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7aab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7aab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7aab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7aab-114">Not supported.</span></span>    |
|<span data-ttu-id="b7aab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7aab-115">Application</span></span> | <span data-ttu-id="b7aab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7aab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7aab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7aab-117">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7aab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7aab-118">Request headers</span></span>
| <span data-ttu-id="b7aab-119">名称</span><span class="sxs-lookup"><span data-stu-id="b7aab-119">Name</span></span>       | <span data-ttu-id="b7aab-120">类型</span><span class="sxs-lookup"><span data-stu-id="b7aab-120">Type</span></span> | <span data-ttu-id="b7aab-121">说明</span><span class="sxs-lookup"><span data-stu-id="b7aab-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b7aab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7aab-122">Authorization</span></span>  | <span data-ttu-id="b7aab-123">string</span><span class="sxs-lookup"><span data-stu-id="b7aab-123">string</span></span>  | <span data-ttu-id="b7aab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7aab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7aab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7aab-126">Request body</span></span>
<span data-ttu-id="b7aab-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7aab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7aab-128">响应</span><span class="sxs-lookup"><span data-stu-id="b7aab-128">Response</span></span>

<span data-ttu-id="b7aab-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b7aab-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="b7aab-130">如果不成功 .。。</span><span class="sxs-lookup"><span data-stu-id="b7aab-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="b7aab-131">示例</span><span class="sxs-lookup"><span data-stu-id="b7aab-131">Example</span></span>
<span data-ttu-id="b7aab-132">下面的示例删除一个策略。</span><span class="sxs-lookup"><span data-stu-id="b7aab-132">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="b7aab-133">请求</span><span class="sxs-lookup"><span data-stu-id="b7aab-133">Request</span></span>
<span data-ttu-id="b7aab-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7aab-134">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="b7aab-135">响应</span><span class="sxs-lookup"><span data-stu-id="b7aab-135">Response</span></span>
<span data-ttu-id="b7aab-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7aab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
