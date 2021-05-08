---
title: 获取 educationSchool
description: 读取 educationSchool 对象的属性和关系。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 21732795ec15c16a92563eccebdeb7e8d33d3793
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231261"
---
# <a name="get-educationschool"></a><span data-ttu-id="f9b1e-103">获取 educationSchool</span><span class="sxs-lookup"><span data-stu-id="f9b1e-103">Get educationSchool</span></span>

<span data-ttu-id="f9b1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9b1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9b1e-105">读取 [educationSchool 对象的属性和](../resources/educationschool.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-105">Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9b1e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f9b1e-106">Permissions</span></span>

<span data-ttu-id="f9b1e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9b1e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9b1e-109">Permission type</span></span>                        | <span data-ttu-id="f9b1e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9b1e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f9b1e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9b1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9b1e-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="f9b1e-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="f9b1e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9b1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9b1e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-114">Not supported.</span></span>                              |
| <span data-ttu-id="f9b1e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9b1e-115">Application</span></span>                            | <span data-ttu-id="f9b1e-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b1e-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9b1e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9b1e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9b1e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9b1e-118">Optional query parameters</span></span>

<span data-ttu-id="f9b1e-119">此方法支持与 Get User 相同的 OData [查询参数](../api/user-get.md#optional-query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-119">This method supports the same OData query parameters as [Get User](../api/user-get.md#optional-query-parameters).</span></span> <span data-ttu-id="f9b1e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9b1e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9b1e-121">Request headers</span></span>

| <span data-ttu-id="f9b1e-122">名称</span><span class="sxs-lookup"><span data-stu-id="f9b1e-122">Name</span></span>          | <span data-ttu-id="f9b1e-123">说明</span><span class="sxs-lookup"><span data-stu-id="f9b1e-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f9b1e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9b1e-124">Authorization</span></span> | <span data-ttu-id="f9b1e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9b1e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9b1e-127">Request body</span></span>

<span data-ttu-id="f9b1e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9b1e-129">响应</span><span class="sxs-lookup"><span data-stu-id="f9b1e-129">Response</span></span>

<span data-ttu-id="f9b1e-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-130">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9b1e-131">示例</span><span class="sxs-lookup"><span data-stu-id="f9b1e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9b1e-132">请求</span><span class="sxs-lookup"><span data-stu-id="f9b1e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```

### <a name="response"></a><span data-ttu-id="f9b1e-133">响应</span><span class="sxs-lookup"><span data-stu-id="f9b1e-133">Response</span></span>

><span data-ttu-id="f9b1e-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f9b1e-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSchool",
    "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
    "displayName": "String",
    "description": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "principalEmail": "String",
    "principalName": "String",
    "externalPrincipalId": "String",
    "lowestGrade": "String",
    "highestGrade": "String",
    "schoolNumber": "String",
    "externalId": "String",
    "phone": "String",
    "fax": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  }
}
```
