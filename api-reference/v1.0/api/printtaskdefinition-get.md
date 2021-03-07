---
title: 获取 taskDefinition
description: 获取有关任务定义的详细信息。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 88f892d511514ecd02e6b8ab10372dfa4de7a2b1
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516945"
---
# <a name="get-printtaskdefinition"></a><span data-ttu-id="18777-103">获取 printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="18777-103">Get printTaskDefinition</span></span>

<span data-ttu-id="18777-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18777-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="18777-105">获取有关任务定义的详细信息。</span><span class="sxs-lookup"><span data-stu-id="18777-105">Get details about a task definition.</span></span>

<span data-ttu-id="18777-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="18777-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="18777-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="18777-107">Permissions</span></span>
<span data-ttu-id="18777-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="18777-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="18777-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="18777-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18777-111">Permission type</span></span> | <span data-ttu-id="18777-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18777-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="18777-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18777-113">Delegated (work or school account)</span></span>| <span data-ttu-id="18777-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18777-114">Not supported.</span></span> |
|<span data-ttu-id="18777-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18777-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18777-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18777-116">Not Supported.</span></span>|
|<span data-ttu-id="18777-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18777-117">Application</span></span>| <span data-ttu-id="18777-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18777-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18777-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18777-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="18777-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18777-120">Request headers</span></span>
|<span data-ttu-id="18777-121">名称</span><span class="sxs-lookup"><span data-stu-id="18777-121">Name</span></span>|<span data-ttu-id="18777-122">说明</span><span class="sxs-lookup"><span data-stu-id="18777-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="18777-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18777-123">Authorization</span></span>|<span data-ttu-id="18777-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18777-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18777-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18777-126">Request body</span></span>
<span data-ttu-id="18777-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18777-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18777-128">响应</span><span class="sxs-lookup"><span data-stu-id="18777-128">Response</span></span>

<span data-ttu-id="18777-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18777-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18777-130">示例</span><span class="sxs-lookup"><span data-stu-id="18777-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18777-131">请求</span><span class="sxs-lookup"><span data-stu-id="18777-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```

### <a name="response"></a><span data-ttu-id="18777-132">响应</span><span class="sxs-lookup"><span data-stu-id="18777-132">Response</span></span>
<span data-ttu-id="18777-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="18777-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

