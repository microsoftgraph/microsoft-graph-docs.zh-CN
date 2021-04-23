---
title: 获取 educationAssignmentSettings
description: 读取 educationAssignmentSettings 对象的属性和关系。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0b49674930f47adb8c4bb9de2a22ef5dfacc565a
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961273"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="3009f-103">获取 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3009f-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="3009f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3009f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3009f-105">读取 [educationAssignmentSettings 对象的属性和](../resources/educationassignmentsettings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3009f-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3009f-106">权限</span><span class="sxs-lookup"><span data-stu-id="3009f-106">Permissions</span></span>
<span data-ttu-id="3009f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3009f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3009f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3009f-109">Permission type</span></span>|<span data-ttu-id="3009f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3009f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3009f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3009f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3009f-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3009f-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="3009f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3009f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3009f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3009f-114">Not supported.</span></span>|
|<span data-ttu-id="3009f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3009f-115">Application</span></span>| <span data-ttu-id="3009f-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3009f-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3009f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3009f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3009f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3009f-118">Optional query parameters</span></span>
<span data-ttu-id="3009f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3009f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3009f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3009f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3009f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3009f-121">Request headers</span></span>
|<span data-ttu-id="3009f-122">名称</span><span class="sxs-lookup"><span data-stu-id="3009f-122">Name</span></span>|<span data-ttu-id="3009f-123">说明</span><span class="sxs-lookup"><span data-stu-id="3009f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3009f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3009f-124">Authorization</span></span>|<span data-ttu-id="3009f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3009f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3009f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3009f-127">Request body</span></span>
<span data-ttu-id="3009f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3009f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3009f-129">响应</span><span class="sxs-lookup"><span data-stu-id="3009f-129">Response</span></span>

<span data-ttu-id="3009f-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3009f-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3009f-131">示例</span><span class="sxs-lookup"><span data-stu-id="3009f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3009f-132">请求</span><span class="sxs-lookup"><span data-stu-id="3009f-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3009f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3009f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="3009f-134">C#</span><span class="sxs-lookup"><span data-stu-id="3009f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3009f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3009f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3009f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3009f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3009f-137">Java</span><span class="sxs-lookup"><span data-stu-id="3009f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3009f-138">响应</span><span class="sxs-lookup"><span data-stu-id="3009f-138">Response</span></span>
<span data-ttu-id="3009f-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3009f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "submissionAnimationDisabled": false
  }
}
```

