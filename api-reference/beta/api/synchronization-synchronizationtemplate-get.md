---
title: 获取 synchronizationTemplate
description: 通过其标识符来检索同步模板。
ms.openlocfilehash: 1ff3f11cf42f5a861e379c8fba2b491fbee2225e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043396"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="79608-103">获取 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="79608-103">Get synchronizationTemplate</span></span>

> <span data-ttu-id="79608-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="79608-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79608-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="79608-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79608-106">通过其标识符来检索同步模板。</span><span class="sxs-lookup"><span data-stu-id="79608-106">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="79608-107">权限</span><span class="sxs-lookup"><span data-stu-id="79608-107">Permissions</span></span>
<span data-ttu-id="79608-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79608-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79608-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79608-110">Permission type</span></span>                        | <span data-ttu-id="79608-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79608-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="79608-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79608-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="79608-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79608-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="79608-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79608-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="79608-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79608-115">Not supported.</span></span>|
|<span data-ttu-id="79608-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79608-116">Application</span></span>                            |<span data-ttu-id="79608-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79608-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="79608-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79608-118">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="79608-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="79608-119">Request headers</span></span>

| <span data-ttu-id="79608-120">名称</span><span class="sxs-lookup"><span data-stu-id="79608-120">Name</span></span>           | <span data-ttu-id="79608-121">类型</span><span class="sxs-lookup"><span data-stu-id="79608-121">Type</span></span>    | <span data-ttu-id="79608-122">说明</span><span class="sxs-lookup"><span data-stu-id="79608-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="79608-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79608-123">Authorization</span></span>  | <span data-ttu-id="79608-124">string</span><span class="sxs-lookup"><span data-stu-id="79608-124">string</span></span>  | <span data-ttu-id="79608-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79608-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79608-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79608-127">Request body</span></span>

<span data-ttu-id="79608-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79608-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="79608-129">响应</span><span class="sxs-lookup"><span data-stu-id="79608-129">Response</span></span>

<span data-ttu-id="79608-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79608-130">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="79608-131">示例</span><span class="sxs-lookup"><span data-stu-id="79608-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="79608-132">请求</span><span class="sxs-lookup"><span data-stu-id="79608-132">Request</span></span>
<span data-ttu-id="79608-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79608-133">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="79608-134">响应</span><span class="sxs-lookup"><span data-stu-id="79608-134">Response</span></span>
<span data-ttu-id="79608-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="79608-135">The following is an example of a response.</span></span>
><span data-ttu-id="79608-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79608-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79608-137">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="79608-137">All the properties will be returned in an actual call.</span></span>

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