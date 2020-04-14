---
title: 获取 synchronizationTemplate
description: 按其标识符检索同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e0f5ff93cc87bd5c4cca2ada9891ba8ce4d02ac4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471158"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="12d5e-103">获取 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="12d5e-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="12d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12d5e-105">按其标识符检索同步模板。</span><span class="sxs-lookup"><span data-stu-id="12d5e-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="12d5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="12d5e-106">Permissions</span></span>
<span data-ttu-id="12d5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12d5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="12d5e-109">Permission type</span></span>                        | <span data-ttu-id="12d5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12d5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="12d5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12d5e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="12d5e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d5e-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="12d5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12d5e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="12d5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12d5e-114">Not supported.</span></span>|
|<span data-ttu-id="12d5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="12d5e-115">Application</span></span>                            |<span data-ttu-id="12d5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12d5e-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="12d5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12d5e-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="12d5e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="12d5e-118">Request headers</span></span>

| <span data-ttu-id="12d5e-119">名称</span><span class="sxs-lookup"><span data-stu-id="12d5e-119">Name</span></span>           | <span data-ttu-id="12d5e-120">类型</span><span class="sxs-lookup"><span data-stu-id="12d5e-120">Type</span></span>    | <span data-ttu-id="12d5e-121">说明</span><span class="sxs-lookup"><span data-stu-id="12d5e-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="12d5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12d5e-122">Authorization</span></span>  | <span data-ttu-id="12d5e-123">string</span><span class="sxs-lookup"><span data-stu-id="12d5e-123">string</span></span>  | <span data-ttu-id="12d5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12d5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12d5e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12d5e-126">Request body</span></span>

<span data-ttu-id="12d5e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12d5e-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="12d5e-128">响应</span><span class="sxs-lookup"><span data-stu-id="12d5e-128">Response</span></span>

<span data-ttu-id="12d5e-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12d5e-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="12d5e-130">示例</span><span class="sxs-lookup"><span data-stu-id="12d5e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="12d5e-131">请求</span><span class="sxs-lookup"><span data-stu-id="12d5e-131">Request</span></span>
<span data-ttu-id="12d5e-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="12d5e-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="12d5e-133">响应</span><span class="sxs-lookup"><span data-stu-id="12d5e-133">Response</span></span>
<span data-ttu-id="12d5e-134">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="12d5e-134">The following is an example of a response.</span></span>
><span data-ttu-id="12d5e-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="12d5e-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="12d5e-136">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="12d5e-136">All the properties will be returned in an actual call.</span></span>

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
