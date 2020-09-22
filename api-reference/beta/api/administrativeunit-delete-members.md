---
title: 删除成员
description: 使用此 API 可从管理单元中删除 (用户或组) 的成员。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d4763a7ab2782b33be6c254f13a852ca8f14787
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991794"
---
# <a name="remove-a-member"></a><span data-ttu-id="0f069-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="0f069-103">Remove a member</span></span>

<span data-ttu-id="0f069-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f069-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f069-105">使用此 API 可从管理单元中删除 (用户或组) 的成员。</span><span class="sxs-lookup"><span data-stu-id="0f069-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f069-106">权限</span><span class="sxs-lookup"><span data-stu-id="0f069-106">Permissions</span></span>
<span data-ttu-id="0f069-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0f069-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f069-109">Permission type</span></span>      | <span data-ttu-id="0f069-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f069-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f069-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f069-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f069-112">AdministrativeUnit、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="0f069-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0f069-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f069-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f069-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f069-114">Not supported.</span></span>    |
|<span data-ttu-id="0f069-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f069-115">Application</span></span> | <span data-ttu-id="0f069-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f069-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f069-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f069-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0f069-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f069-118">Request headers</span></span>
| <span data-ttu-id="0f069-119">名称</span><span class="sxs-lookup"><span data-stu-id="0f069-119">Name</span></span>      |<span data-ttu-id="0f069-120">说明</span><span class="sxs-lookup"><span data-stu-id="0f069-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0f069-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f069-121">Authorization</span></span>  | <span data-ttu-id="0f069-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f069-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f069-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f069-124">Request body</span></span>
<span data-ttu-id="0f069-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f069-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f069-126">响应</span><span class="sxs-lookup"><span data-stu-id="0f069-126">Response</span></span>

<span data-ttu-id="0f069-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0f069-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f069-129">示例</span><span class="sxs-lookup"><span data-stu-id="0f069-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f069-130">请求</span><span class="sxs-lookup"><span data-stu-id="0f069-130">Request</span></span>
<span data-ttu-id="0f069-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f069-131">Here is an example of the request.</span></span> <span data-ttu-id="0f069-132">在下面的示例中，id1 表示目标管理单元的标识符，id2 表示要从目标管理单元中删除的成员用户或组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0f069-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="0f069-133">响应</span><span class="sxs-lookup"><span data-stu-id="0f069-133">Response</span></span>
<span data-ttu-id="0f069-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f069-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```


