---
title: educationSchool： delta
description: 获取新创建或更新的学校，而无需对整个学校集合执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5e436f7061043a1cab5a3d92c3401f4949a08782
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909525"
---
# <a name="educationschool-delta"></a><span data-ttu-id="0d744-103">educationSchool： delta</span><span class="sxs-lookup"><span data-stu-id="0d744-103">educationSchool: delta</span></span>

<span data-ttu-id="0d744-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d744-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d744-105">获取新创建或更新的学校，而无需对整个学校集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="0d744-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="0d744-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="0d744-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d744-107">权限</span><span class="sxs-lookup"><span data-stu-id="0d744-107">Permissions</span></span>

<span data-ttu-id="0d744-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0d744-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0d744-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d744-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d744-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d744-110">Permission type</span></span>                        | <span data-ttu-id="0d744-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d744-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="0d744-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d744-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d744-113">Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all</span><span class="sxs-lookup"><span data-stu-id="0d744-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="0d744-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d744-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d744-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d744-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="0d744-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d744-116">Application</span></span>                            | <span data-ttu-id="0d744-117">Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="0d744-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d744-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d744-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a><span data-ttu-id="0d744-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d744-119">Request headers</span></span>

| <span data-ttu-id="0d744-120">名称</span><span class="sxs-lookup"><span data-stu-id="0d744-120">Name</span></span>          | <span data-ttu-id="0d744-121">说明</span><span class="sxs-lookup"><span data-stu-id="0d744-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="0d744-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d744-122">Authorization</span></span> | <span data-ttu-id="0d744-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0d744-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d744-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d744-124">Request body</span></span>

<span data-ttu-id="0d744-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d744-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d744-126">响应</span><span class="sxs-lookup"><span data-stu-id="0d744-126">Response</span></span>

<span data-ttu-id="0d744-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[educationSchool](../resources/educationschool.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="0d744-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0d744-128">educationSchool 增量不包括已删除的学校。</span><span class="sxs-lookup"><span data-stu-id="0d744-128">educationSchool deltas do not include deleted schools.</span></span>

## <a name="example"></a><span data-ttu-id="0d744-129">示例</span><span class="sxs-lookup"><span data-stu-id="0d744-129">Example</span></span>

<span data-ttu-id="0d744-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0d744-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0d744-131">请求</span><span class="sxs-lookup"><span data-stu-id="0d744-131">Request</span></span>

<span data-ttu-id="0d744-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d744-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="0d744-133">响应</span><span class="sxs-lookup"><span data-stu-id="0d744-133">Response</span></span>

<span data-ttu-id="0d744-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d744-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0d744-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0d744-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0d744-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0d744-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
