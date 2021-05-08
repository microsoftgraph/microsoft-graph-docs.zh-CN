---
title: educationUser： delta
description: 获取新创建或更新的用户，而无需执行整个用户集合的完全读取。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eddf1656a9f1366276b89fd5b101768b45e2cca1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232134"
---
# <a name="educationuser-delta"></a><span data-ttu-id="d5772-103">educationUser： delta</span><span class="sxs-lookup"><span data-stu-id="d5772-103">educationUser: delta</span></span>

<span data-ttu-id="d5772-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5772-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5772-105">获取新创建或更新的 [educationUser，](../resources/educationuser.md) 而无需执行整个集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="d5772-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="d5772-106">有关详细信息 [，请参阅使用 delta](/graph/delta-query-overview) 查询。</span><span class="sxs-lookup"><span data-stu-id="d5772-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5772-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5772-107">Permissions</span></span>

<span data-ttu-id="d5772-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5772-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5772-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5772-110">Permission type</span></span>                        | <span data-ttu-id="d5772-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5772-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d5772-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5772-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5772-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d5772-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="d5772-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5772-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5772-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5772-115">Not supported.</span></span>                              |
| <span data-ttu-id="d5772-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5772-116">Application</span></span>                            | <span data-ttu-id="d5772-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5772-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5772-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5772-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="d5772-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5772-119">Request headers</span></span>

| <span data-ttu-id="d5772-120">名称</span><span class="sxs-lookup"><span data-stu-id="d5772-120">Name</span></span>          | <span data-ttu-id="d5772-121">说明</span><span class="sxs-lookup"><span data-stu-id="d5772-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d5772-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5772-122">Authorization</span></span> | <span data-ttu-id="d5772-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5772-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5772-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5772-125">Request body</span></span>

<span data-ttu-id="d5772-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5772-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5772-127">响应</span><span class="sxs-lookup"><span data-stu-id="d5772-127">Response</span></span>

<span data-ttu-id="d5772-128">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [educationUser](../resources/educationuser.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d5772-128">If successful, this function returns a `200 OK` response code and a [educationUser](../resources/educationuser.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5772-129">示例</span><span class="sxs-lookup"><span data-stu-id="d5772-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5772-130">请求</span><span class="sxs-lookup"><span data-stu-id="d5772-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users/delta
```

### <a name="response"></a><span data-ttu-id="d5772-131">响应</span><span class="sxs-lookup"><span data-stu-id="d5772-131">Response</span></span>

> <span data-ttu-id="d5772-132">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d5772-132">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationUser)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationUser)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/users/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "String (identifier)",
      "primaryRole": "String",
      "middleName": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "mailingAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "student": {
        "@odata.type": "microsoft.graph.educationStudent"
      },
      "teacher": {
        "@odata.type": "microsoft.graph.educationTeacher"
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "accountEnabled": "Boolean",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "department": "String",
      "displayName": "String",
      "givenName": "String",
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      }
    }
  ]
}
```
