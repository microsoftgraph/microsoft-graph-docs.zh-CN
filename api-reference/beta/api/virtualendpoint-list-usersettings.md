---
title: 列出 userSettings
description: 检索 cloudPcUserSetting 对象的列表。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6d953baaf3d071ca999031bfd5ae07dcfe378106
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993652"
---
# <a name="list-usersettings"></a><span data-ttu-id="73c34-103">列出 userSettings</span><span class="sxs-lookup"><span data-stu-id="73c34-103">List userSettings</span></span>

<span data-ttu-id="73c34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73c34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73c34-105">检索 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="73c34-105">Retrieve a list of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="73c34-106">权限</span><span class="sxs-lookup"><span data-stu-id="73c34-106">Permissions</span></span>

<span data-ttu-id="73c34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73c34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73c34-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73c34-109">Permission type</span></span>|<span data-ttu-id="73c34-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73c34-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73c34-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73c34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73c34-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c34-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="73c34-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73c34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73c34-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73c34-114">Not supported.</span></span>|
|<span data-ttu-id="73c34-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73c34-115">Application</span></span>|<span data-ttu-id="73c34-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c34-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73c34-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73c34-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73c34-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73c34-118">Optional query parameters</span></span>

<span data-ttu-id="73c34-119">此方法支持 `$select` 、 `$filter` 和 `$expand` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73c34-119">This method the supports `$select`, `$filter`, and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="73c34-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="73c34-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="73c34-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="73c34-121">Request headers</span></span>

| <span data-ttu-id="73c34-122">名称</span><span class="sxs-lookup"><span data-stu-id="73c34-122">Name</span></span>          | <span data-ttu-id="73c34-123">说明</span><span class="sxs-lookup"><span data-stu-id="73c34-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="73c34-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="73c34-124">Authorization</span></span> | <span data-ttu-id="73c34-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73c34-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73c34-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73c34-127">Request body</span></span>

<span data-ttu-id="73c34-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73c34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73c34-129">响应</span><span class="sxs-lookup"><span data-stu-id="73c34-129">Response</span></span>

<span data-ttu-id="73c34-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="73c34-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73c34-131">示例</span><span class="sxs-lookup"><span data-stu-id="73c34-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73c34-132">请求</span><span class="sxs-lookup"><span data-stu-id="73c34-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
```


### <a name="response"></a><span data-ttu-id="73c34-133">响应</span><span class="sxs-lookup"><span data-stu-id="73c34-133">Response</span></span>
><span data-ttu-id="73c34-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="73c34-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcUserSetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcUserSetting",
      "id": "556092f8-92f8-5560-f892-6055f8926055",
      "displayName": "Test1",
      "selfServiceEnabled": true,
      "localAdminEnabled": false,
      "lastModifiedDateTime": "2021-02-01T10:29:57Z",
      "createdDateTime": "2021-02-01T10:29:57Z"
    }
  ]
}
```
