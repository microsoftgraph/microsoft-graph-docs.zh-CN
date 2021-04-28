---
title: 获取部署
description: 读取部署对象的属性和关系。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 43081598030efc8ac4b3e30fe35d99931dde5d8f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067840"
---
# <a name="get-deployment"></a><span data-ttu-id="c753f-103">获取部署</span><span class="sxs-lookup"><span data-stu-id="c753f-103">Get deployment</span></span>
<span data-ttu-id="c753f-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c753f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c753f-105">读取部署 [对象的属性和](../resources/windowsupdates-deployment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c753f-105">Read the properties and relationships of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c753f-106">权限</span><span class="sxs-lookup"><span data-stu-id="c753f-106">Permissions</span></span>
<span data-ttu-id="c753f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c753f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c753f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c753f-109">Permission type</span></span>|<span data-ttu-id="c753f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c753f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c753f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c753f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c753f-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c753f-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c753f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c753f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c753f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c753f-114">Not supported.</span></span>|
|<span data-ttu-id="c753f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c753f-115">Application</span></span>|<span data-ttu-id="c753f-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c753f-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c753f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c753f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c753f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c753f-118">Optional query parameters</span></span>
<span data-ttu-id="c753f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c753f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c753f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c753f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c753f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c753f-121">Request headers</span></span>
|<span data-ttu-id="c753f-122">名称</span><span class="sxs-lookup"><span data-stu-id="c753f-122">Name</span></span>|<span data-ttu-id="c753f-123">说明</span><span class="sxs-lookup"><span data-stu-id="c753f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c753f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c753f-124">Authorization</span></span>|<span data-ttu-id="c753f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c753f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c753f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c753f-127">Request body</span></span>
<span data-ttu-id="c753f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c753f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c753f-129">响应</span><span class="sxs-lookup"><span data-stu-id="c753f-129">Response</span></span>

<span data-ttu-id="c753f-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/windowsupdates-deployment.md)代码和部署对象。</span><span class="sxs-lookup"><span data-stu-id="c753f-130">If successful, this method returns a `200 OK` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c753f-131">示例</span><span class="sxs-lookup"><span data-stu-id="c753f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c753f-132">请求</span><span class="sxs-lookup"><span data-stu-id="c753f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
```


### <a name="response"></a><span data-ttu-id="c753f-133">响应</span><span class="sxs-lookup"><span data-stu-id="c753f-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
    },
    "content": {
      "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
    },
    "settings": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

