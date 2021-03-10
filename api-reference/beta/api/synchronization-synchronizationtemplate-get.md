---
title: 获取 synchronizationTemplate
description: 按同步模板的标识符检索同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6d4663d4b6ed7275c00f61f0e1a93f13f2b1e0bf
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625927"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="c2836-103">获取 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="c2836-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="c2836-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2836-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2836-105">按同步模板的标识符检索同步模板。</span><span class="sxs-lookup"><span data-stu-id="c2836-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2836-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2836-106">Permissions</span></span>
<span data-ttu-id="c2836-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2836-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2836-109">Permission type</span></span>                        | <span data-ttu-id="c2836-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2836-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2836-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2836-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="c2836-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2836-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="c2836-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2836-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c2836-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2836-114">Not supported.</span></span>|
|<span data-ttu-id="c2836-115">Application</span><span class="sxs-lookup"><span data-stu-id="c2836-115">Application</span></span>                            |<span data-ttu-id="c2836-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2836-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="c2836-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2836-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="c2836-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2836-118">Request headers</span></span>

| <span data-ttu-id="c2836-119">名称</span><span class="sxs-lookup"><span data-stu-id="c2836-119">Name</span></span>           | <span data-ttu-id="c2836-120">类型</span><span class="sxs-lookup"><span data-stu-id="c2836-120">Type</span></span>    | <span data-ttu-id="c2836-121">说明</span><span class="sxs-lookup"><span data-stu-id="c2836-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c2836-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2836-122">Authorization</span></span>  | <span data-ttu-id="c2836-123">string</span><span class="sxs-lookup"><span data-stu-id="c2836-123">string</span></span>  | <span data-ttu-id="c2836-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2836-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2836-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2836-126">Request body</span></span>

<span data-ttu-id="c2836-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2836-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="c2836-128">响应</span><span class="sxs-lookup"><span data-stu-id="c2836-128">Response</span></span>

<span data-ttu-id="c2836-129">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2836-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="c2836-130">示例</span><span class="sxs-lookup"><span data-stu-id="c2836-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2836-131">请求</span><span class="sxs-lookup"><span data-stu-id="c2836-131">Request</span></span>
<span data-ttu-id="c2836-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c2836-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="c2836-133">响应</span><span class="sxs-lookup"><span data-stu-id="c2836-133">Response</span></span>
<span data-ttu-id="c2836-134">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c2836-134">The following is an example of a response.</span></span>
><span data-ttu-id="c2836-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c2836-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c2836-136">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2836-136">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```


