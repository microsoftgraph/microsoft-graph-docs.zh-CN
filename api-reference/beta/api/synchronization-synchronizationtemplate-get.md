---
title: 获取 synchronizationTemplate
description: 按其标识符检索同步模板。
localization_priority: Normal
ms.openlocfilehash: 982727fa54f1b6f83d7acf382f0ccacdad72b7ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335542"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="3b580-103">获取 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="3b580-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b580-104">按其标识符检索同步模板。</span><span class="sxs-lookup"><span data-stu-id="3b580-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b580-105">权限</span><span class="sxs-lookup"><span data-stu-id="3b580-105">Permissions</span></span>
<span data-ttu-id="3b580-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b580-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b580-108">Permission type</span></span>                        | <span data-ttu-id="3b580-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b580-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b580-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b580-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="3b580-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b580-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3b580-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b580-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3b580-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b580-113">Not supported.</span></span>|
|<span data-ttu-id="3b580-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b580-114">Application</span></span>                            |<span data-ttu-id="3b580-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b580-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="3b580-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b580-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="3b580-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b580-117">Request headers</span></span>

| <span data-ttu-id="3b580-118">名称</span><span class="sxs-lookup"><span data-stu-id="3b580-118">Name</span></span>           | <span data-ttu-id="3b580-119">类型</span><span class="sxs-lookup"><span data-stu-id="3b580-119">Type</span></span>    | <span data-ttu-id="3b580-120">说明</span><span class="sxs-lookup"><span data-stu-id="3b580-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3b580-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b580-121">Authorization</span></span>  | <span data-ttu-id="3b580-122">string</span><span class="sxs-lookup"><span data-stu-id="3b580-122">string</span></span>  | <span data-ttu-id="3b580-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b580-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b580-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b580-125">Request body</span></span>

<span data-ttu-id="3b580-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b580-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="3b580-127">响应</span><span class="sxs-lookup"><span data-stu-id="3b580-127">Response</span></span>

<span data-ttu-id="3b580-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b580-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="3b580-129">示例</span><span class="sxs-lookup"><span data-stu-id="3b580-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3b580-130">请求</span><span class="sxs-lookup"><span data-stu-id="3b580-130">Request</span></span>
<span data-ttu-id="3b580-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3b580-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="3b580-132">响应</span><span class="sxs-lookup"><span data-stu-id="3b580-132">Response</span></span>
<span data-ttu-id="3b580-133">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3b580-133">The following is an example of a response.</span></span>
><span data-ttu-id="3b580-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3b580-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3b580-135">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="3b580-135">All the properties will be returned in an actual call.</span></span>

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
