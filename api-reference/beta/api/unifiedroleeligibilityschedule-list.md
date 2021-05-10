---
title: 列出 unifiedRoleEligibilitySchedules
description: 获取 unifiedRoleEligibilitySchedule 对象及其属性的列表。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6d4a2c4ad3475b0f5a6a12f43248213cf3cf56af
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299125"
---
# <a name="list-unifiedroleeligibilityschedules"></a><span data-ttu-id="e64e5-103">列出 unifiedRoleEligibilitySchedules</span><span class="sxs-lookup"><span data-stu-id="e64e5-103">List unifiedRoleEligibilitySchedules</span></span>
<span data-ttu-id="e64e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e64e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e64e5-105">获取 [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e64e5-105">Get a list of the [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e64e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="e64e5-106">Permissions</span></span>
<span data-ttu-id="e64e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e64e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e64e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e64e5-109">Permission type</span></span>|<span data-ttu-id="e64e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e64e5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e64e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e64e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e64e5-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e64e5-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="e64e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e64e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e64e5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="e64e5-114">Not supported</span></span>|
|<span data-ttu-id="e64e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e64e5-115">Application</span></span>|<span data-ttu-id="e64e5-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e64e5-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="e64e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e64e5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e64e5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e64e5-118">Optional query parameters</span></span>
<span data-ttu-id="e64e5-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e64e5-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e64e5-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e64e5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e64e5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e64e5-121">Request headers</span></span>
|<span data-ttu-id="e64e5-122">名称</span><span class="sxs-lookup"><span data-stu-id="e64e5-122">Name</span></span>|<span data-ttu-id="e64e5-123">说明</span><span class="sxs-lookup"><span data-stu-id="e64e5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e64e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e64e5-124">Authorization</span></span>|<span data-ttu-id="e64e5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e64e5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e64e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e64e5-127">Request body</span></span>
<span data-ttu-id="e64e5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e64e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e64e5-129">响应</span><span class="sxs-lookup"><span data-stu-id="e64e5-129">Response</span></span>

<span data-ttu-id="e64e5-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e64e5-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e64e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="e64e5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e64e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="e64e5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules
```


### <a name="response"></a><span data-ttu-id="e64e5-133">响应</span><span class="sxs-lookup"><span data-stu-id="e64e5-133">Response</span></span>
<span data-ttu-id="e64e5-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e64e5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdUsing": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "memberType": "direct"
    }
  ]
}
```

