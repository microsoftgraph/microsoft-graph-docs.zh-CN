---
title: 获取 educationAssignmentDefaults
description: 读取 educationAssignmentDefaults 对象的属性和关系。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c99f43ee19b40c0223d94ac4b9519b55bddcfcd3
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991230"
---
# <a name="get-educationassignmentdefaults"></a><span data-ttu-id="5a724-103">获取 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="5a724-103">Get educationAssignmentDefaults</span></span>
<span data-ttu-id="5a724-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a724-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a724-105">读取 [educationAssignmentDefaults 对象的属性和](../resources/educationassignmentdefaults.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="5a724-105">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> 

<span data-ttu-id="5a724-106">这些是类中新建的工作分配所遵守的类级别分配默认值。</span><span class="sxs-lookup"><span data-stu-id="5a724-106">These are the class-level assignment defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="5a724-107">如果调用方不希望使用默认行为，可以继续为每个工作分配创建指定自定义值。</span><span class="sxs-lookup"><span data-stu-id="5a724-107">Callers can continue to specify custom values on each assignment creation if they Don't want the default behaviors.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a724-108">权限</span><span class="sxs-lookup"><span data-stu-id="5a724-108">Permissions</span></span>
<span data-ttu-id="5a724-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a724-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a724-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a724-111">Permission type</span></span>|<span data-ttu-id="5a724-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a724-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a724-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a724-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5a724-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a724-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="5a724-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a724-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5a724-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a724-116">Not supported.</span></span> |
|<span data-ttu-id="5a724-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a724-117">Application</span></span>| <span data-ttu-id="5a724-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a724-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a724-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a724-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a724-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a724-120">Optional query parameters</span></span>
<span data-ttu-id="5a724-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5a724-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5a724-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5a724-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a724-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a724-123">Request headers</span></span>
|<span data-ttu-id="5a724-124">名称</span><span class="sxs-lookup"><span data-stu-id="5a724-124">Name</span></span>|<span data-ttu-id="5a724-125">说明</span><span class="sxs-lookup"><span data-stu-id="5a724-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5a724-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a724-126">Authorization</span></span>|<span data-ttu-id="5a724-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a724-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a724-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a724-129">Request body</span></span>
<span data-ttu-id="5a724-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a724-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a724-131">响应</span><span class="sxs-lookup"><span data-stu-id="5a724-131">Response</span></span>

<span data-ttu-id="5a724-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a724-132">If successful, this method returns a `200 OK` response code and an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a724-133">示例</span><span class="sxs-lookup"><span data-stu-id="5a724-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a724-134">请求</span><span class="sxs-lookup"><span data-stu-id="5a724-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5a724-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a724-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentdefaults"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```
# <a name="c"></a>[<span data-ttu-id="5a724-136">C#</span><span class="sxs-lookup"><span data-stu-id="5a724-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a724-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a724-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a724-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a724-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a724-139">Java</span><span class="sxs-lookup"><span data-stu-id="5a724-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5a724-140">响应</span><span class="sxs-lookup"><span data-stu-id="5a724-140">Response</span></span>
<span data-ttu-id="5a724-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a724-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "addedStudentAction": "none",
    "dueTime": "23:59:00",
    "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('c6f4e171-da1f-4598-a648-05fcec6cd9ba')"
  }
}
```

