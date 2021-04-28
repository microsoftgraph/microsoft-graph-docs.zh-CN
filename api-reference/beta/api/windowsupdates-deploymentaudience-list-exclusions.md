---
title: 列出部署访问群体排除项
description: 列出从 deploymentAudience 中排除的 updatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6f65aa86694478a545c236b7cd4f54a9468bb601
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067315"
---
# <a name="list-deployment-audience-exclusions"></a><span data-ttu-id="baa30-103">列出部署访问群体排除项</span><span class="sxs-lookup"><span data-stu-id="baa30-103">List deployment audience exclusions</span></span>
<span data-ttu-id="baa30-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="baa30-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baa30-105">列出从[deploymentAudience](../resources/windowsupdates-deploymentaudience.md)中排除的[updatableAsset](../resources/windowsupdates-updatableasset.md)资源。</span><span class="sxs-lookup"><span data-stu-id="baa30-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are excluded from a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="baa30-106">权限</span><span class="sxs-lookup"><span data-stu-id="baa30-106">Permissions</span></span>
<span data-ttu-id="baa30-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baa30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baa30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="baa30-109">Permission type</span></span>|<span data-ttu-id="baa30-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baa30-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baa30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baa30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="baa30-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa30-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="baa30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baa30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baa30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="baa30-114">Not supported.</span></span>|
|<span data-ttu-id="baa30-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="baa30-115">Application</span></span>|<span data-ttu-id="baa30-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa30-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="baa30-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baa30-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/exclusions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="baa30-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="baa30-118">Optional query parameters</span></span>
<span data-ttu-id="baa30-119">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="baa30-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="baa30-120">若要对不是从 [updatableAsset](../resources/windowsupdates-updatableasset.md)继承的属性使用查询参数，请包含属性的完整资源类型。</span><span class="sxs-lookup"><span data-stu-id="baa30-120">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="baa30-121">例如，若要选择 [azureADDevice，](../resources/windowsupdates-azureaddevice.md) `errors` 请使用 `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` 。</span><span class="sxs-lookup"><span data-stu-id="baa30-121">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="baa30-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="baa30-122">Request headers</span></span>
|<span data-ttu-id="baa30-123">名称</span><span class="sxs-lookup"><span data-stu-id="baa30-123">Name</span></span>|<span data-ttu-id="baa30-124">说明</span><span class="sxs-lookup"><span data-stu-id="baa30-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="baa30-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="baa30-125">Authorization</span></span>|<span data-ttu-id="baa30-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="baa30-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="baa30-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="baa30-128">Request body</span></span>
<span data-ttu-id="baa30-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="baa30-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baa30-130">响应</span><span class="sxs-lookup"><span data-stu-id="baa30-130">Response</span></span>

<span data-ttu-id="baa30-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="baa30-131">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="baa30-132">示例</span><span class="sxs-lookup"><span data-stu-id="baa30-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="baa30-133">请求</span><span class="sxs-lookup"><span data-stu-id="baa30-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/exclusions
```


### <a name="response"></a><span data-ttu-id="baa30-134">响应</span><span class="sxs-lookup"><span data-stu-id="baa30-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "fb95f07d-9e73-411d-99ab-7eca3a5122b1",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
        }
      ]
    },
  ]
}
```

