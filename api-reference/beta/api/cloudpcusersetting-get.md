---
title: 获取 cloudPcUserSetting
description: 读取 cloudPcUserSetting 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b54797490580a4f1bda43252aed726292884b6a0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993642"
---
# <a name="get-cloudpcusersetting"></a><span data-ttu-id="60d9a-103">获取 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="60d9a-103">Get cloudPcUserSetting</span></span>

<span data-ttu-id="60d9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60d9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60d9a-105">读取 [cloudPcUserSetting 对象的属性和](../resources/cloudpcusersetting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="60d9a-105">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="60d9a-106">权限</span><span class="sxs-lookup"><span data-stu-id="60d9a-106">Permissions</span></span>

<span data-ttu-id="60d9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60d9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d9a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60d9a-109">Permission type</span></span>|<span data-ttu-id="60d9a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60d9a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60d9a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60d9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60d9a-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d9a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="60d9a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60d9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60d9a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="60d9a-114">Not supported.</span></span>|
|<span data-ttu-id="60d9a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="60d9a-115">Application</span></span>|<span data-ttu-id="60d9a-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d9a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60d9a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60d9a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60d9a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="60d9a-118">Optional query parameters</span></span>

<span data-ttu-id="60d9a-119">此方法支持 `$select` `$expand` 和 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="60d9a-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="60d9a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="60d9a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60d9a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="60d9a-121">Request headers</span></span>

| <span data-ttu-id="60d9a-122">名称</span><span class="sxs-lookup"><span data-stu-id="60d9a-122">Name</span></span>          | <span data-ttu-id="60d9a-123">说明</span><span class="sxs-lookup"><span data-stu-id="60d9a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="60d9a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="60d9a-124">Authorization</span></span> | <span data-ttu-id="60d9a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60d9a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60d9a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60d9a-127">Request body</span></span>

<span data-ttu-id="60d9a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60d9a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60d9a-129">响应</span><span class="sxs-lookup"><span data-stu-id="60d9a-129">Response</span></span>

<span data-ttu-id="60d9a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60d9a-130">If successful, this method returns a `200 OK` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60d9a-131">示例</span><span class="sxs-lookup"><span data-stu-id="60d9a-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-user-setting"></a><span data-ttu-id="60d9a-132">示例 1：获取指定用户设置的属性</span><span class="sxs-lookup"><span data-stu-id="60d9a-132">Example 1: Get the properties of the specified user setting</span></span>

#### <a name="request"></a><span data-ttu-id="60d9a-133">请求</span><span class="sxs-lookup"><span data-stu-id="60d9a-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055
```


#### <a name="response"></a><span data-ttu-id="60d9a-134">响应</span><span class="sxs-lookup"><span data-stu-id="60d9a-134">Response</span></span>
><span data-ttu-id="60d9a-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="60d9a-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "556092f8-92f8-5560-f892-6055f8926055",
    "displayName": "String",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-user-setting-and-expand-on-the-assignments"></a><span data-ttu-id="60d9a-136">示例 2：获取指定用户设置的属性，然后展开工作分配</span><span class="sxs-lookup"><span data-stu-id="60d9a-136">Example 2: Get the properties of the specified user setting and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="60d9a-137">请求</span><span class="sxs-lookup"><span data-stu-id="60d9a-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments
```


#### <a name="response"></a><span data-ttu-id="60d9a-138">响应</span><span class="sxs-lookup"><span data-stu-id="60d9a-138">Response</span></span>

<span data-ttu-id="60d9a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="60d9a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "createdDateTime": "2021-02-01T10:29:57Z",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
