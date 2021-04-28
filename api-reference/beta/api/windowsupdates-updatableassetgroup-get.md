---
title: 获取 updatableAssetGroup
description: 读取 updatableAssetGroup 对象的属性和关系。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6c31b6cb7080f053313513c60639a2d97fe1b0b9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068009"
---
# <a name="get-updatableassetgroup"></a><span data-ttu-id="0c997-103">获取 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="0c997-103">Get updatableAssetGroup</span></span>
<span data-ttu-id="0c997-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="0c997-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c997-105">读取 [updatableAssetGroup 对象的属性和](../resources/windowsupdates-updatableassetgroup.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0c997-105">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c997-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c997-106">Permissions</span></span>
<span data-ttu-id="0c997-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c997-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c997-109">Permission type</span></span>|<span data-ttu-id="0c997-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c997-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c997-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c997-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0c997-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c997-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="0c997-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c997-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c997-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c997-114">Not supported.</span></span>|
|<span data-ttu-id="0c997-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c997-115">Application</span></span>|<span data-ttu-id="0c997-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c997-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c997-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c997-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c997-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c997-118">Optional query parameters</span></span>
<span data-ttu-id="0c997-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c997-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0c997-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0c997-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c997-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c997-121">Request headers</span></span>
|<span data-ttu-id="0c997-122">名称</span><span class="sxs-lookup"><span data-stu-id="0c997-122">Name</span></span>|<span data-ttu-id="0c997-123">说明</span><span class="sxs-lookup"><span data-stu-id="0c997-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c997-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c997-124">Authorization</span></span>|<span data-ttu-id="0c997-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c997-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c997-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c997-127">Request body</span></span>
<span data-ttu-id="0c997-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c997-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c997-129">响应</span><span class="sxs-lookup"><span data-stu-id="0c997-129">Response</span></span>

<span data-ttu-id="0c997-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c997-130">If successful, this method returns a `200 OK` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c997-131">示例</span><span class="sxs-lookup"><span data-stu-id="0c997-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c997-132">请求</span><span class="sxs-lookup"><span data-stu-id="0c997-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c
```


### <a name="response"></a><span data-ttu-id="0c997-133">响应</span><span class="sxs-lookup"><span data-stu-id="0c997-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
    "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
  }
}
```

