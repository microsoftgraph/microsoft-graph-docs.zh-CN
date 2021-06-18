---
title: 更新 educationAssignmentSettings
description: 更新 educationAssignmentSettings 对象的属性。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7c251885de43022f8e3065c7004dab33d4fa78a8
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992969"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="8a093-103">更新 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="8a093-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="8a093-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a093-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a093-105">更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8a093-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="8a093-106">只有教师可以更新这些设置。</span><span class="sxs-lookup"><span data-stu-id="8a093-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a093-107">权限</span><span class="sxs-lookup"><span data-stu-id="8a093-107">Permissions</span></span>
<span data-ttu-id="8a093-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a093-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a093-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a093-110">Permission type</span></span>|<span data-ttu-id="8a093-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a093-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a093-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a093-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a093-113">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a093-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="8a093-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a093-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a093-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a093-115">Not supported.</span></span>|
|<span data-ttu-id="8a093-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a093-116">Application</span></span>|<span data-ttu-id="8a093-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a093-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a093-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a093-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="8a093-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a093-119">Request headers</span></span>
|<span data-ttu-id="8a093-120">名称</span><span class="sxs-lookup"><span data-stu-id="8a093-120">Name</span></span>|<span data-ttu-id="8a093-121">说明</span><span class="sxs-lookup"><span data-stu-id="8a093-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a093-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a093-122">Authorization</span></span>|<span data-ttu-id="8a093-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a093-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a093-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a093-125">Content-Type</span></span>|<span data-ttu-id="8a093-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8a093-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a093-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a093-128">Request body</span></span>
<span data-ttu-id="8a093-129">在请求正文中，提供 [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a093-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="8a093-130">下表显示更新 [educationAssignmentSettings 时所需的属性](../resources/educationassignmentsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="8a093-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="8a093-131">属性</span><span class="sxs-lookup"><span data-stu-id="8a093-131">Property</span></span>|<span data-ttu-id="8a093-132">类型</span><span class="sxs-lookup"><span data-stu-id="8a093-132">Type</span></span>|<span data-ttu-id="8a093-133">说明</span><span class="sxs-lookup"><span data-stu-id="8a093-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a093-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="8a093-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="8a093-135">布尔</span><span class="sxs-lookup"><span data-stu-id="8a093-135">Boolean</span></span>|<span data-ttu-id="8a093-136">指示是否显示打开的庆祝动画。</span><span class="sxs-lookup"><span data-stu-id="8a093-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="8a093-137">的值 `true` 指示不会显示动画。</span><span class="sxs-lookup"><span data-stu-id="8a093-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="8a093-138">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="8a093-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="8a093-139">响应</span><span class="sxs-lookup"><span data-stu-id="8a093-139">Response</span></span>

<span data-ttu-id="8a093-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a093-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a093-141">示例</span><span class="sxs-lookup"><span data-stu-id="8a093-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a093-142">请求</span><span class="sxs-lookup"><span data-stu-id="8a093-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8a093-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a093-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="8a093-144">C#</span><span class="sxs-lookup"><span data-stu-id="8a093-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a093-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a093-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a093-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a093-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a093-147">Java</span><span class="sxs-lookup"><span data-stu-id="8a093-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8a093-148">响应</span><span class="sxs-lookup"><span data-stu-id="8a093-148">Response</span></span>
<span data-ttu-id="8a093-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8a093-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "submissionAnimationDisabled": true
}
```

