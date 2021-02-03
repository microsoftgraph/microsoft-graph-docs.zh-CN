---
title: 更新 educationAssignmentSettings
description: 更新 educationAssignmentSettings 对象的属性。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ec19c4e3f49c5535e6ed5f4eddafbbf21d5428ee
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092497"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="e1db7-103">更新 educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e1db7-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="e1db7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1db7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1db7-105">更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e1db7-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="e1db7-106">只有教师可以更新这些设置。</span><span class="sxs-lookup"><span data-stu-id="e1db7-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1db7-107">权限</span><span class="sxs-lookup"><span data-stu-id="e1db7-107">Permissions</span></span>
<span data-ttu-id="e1db7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1db7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1db7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1db7-110">Permission type</span></span>|<span data-ttu-id="e1db7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1db7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1db7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1db7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1db7-113">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1db7-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="e1db7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1db7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1db7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1db7-115">Not supported.</span></span>|
|<span data-ttu-id="e1db7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1db7-116">Application</span></span>|<span data-ttu-id="e1db7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1db7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1db7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1db7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="e1db7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1db7-119">Request headers</span></span>
|<span data-ttu-id="e1db7-120">名称</span><span class="sxs-lookup"><span data-stu-id="e1db7-120">Name</span></span>|<span data-ttu-id="e1db7-121">说明</span><span class="sxs-lookup"><span data-stu-id="e1db7-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e1db7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1db7-122">Authorization</span></span>|<span data-ttu-id="e1db7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1db7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e1db7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1db7-125">Content-Type</span></span>|<span data-ttu-id="e1db7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e1db7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1db7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1db7-128">Request body</span></span>
<span data-ttu-id="e1db7-129">在请求正文中，提供 [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1db7-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="e1db7-130">下表显示更新 [educationAssignmentSettings 时所需的属性](../resources/educationassignmentsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="e1db7-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="e1db7-131">属性</span><span class="sxs-lookup"><span data-stu-id="e1db7-131">Property</span></span>|<span data-ttu-id="e1db7-132">类型</span><span class="sxs-lookup"><span data-stu-id="e1db7-132">Type</span></span>|<span data-ttu-id="e1db7-133">Description</span><span class="sxs-lookup"><span data-stu-id="e1db7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1db7-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="e1db7-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="e1db7-135">布尔</span><span class="sxs-lookup"><span data-stu-id="e1db7-135">Boolean</span></span>|<span data-ttu-id="e1db7-136">指示是否显示打开的庆祝动画。</span><span class="sxs-lookup"><span data-stu-id="e1db7-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="e1db7-137">值 `true` 指示不会显示动画。</span><span class="sxs-lookup"><span data-stu-id="e1db7-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="e1db7-138">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e1db7-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="e1db7-139">响应</span><span class="sxs-lookup"><span data-stu-id="e1db7-139">Response</span></span>

<span data-ttu-id="e1db7-140">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1db7-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1db7-141">示例</span><span class="sxs-lookup"><span data-stu-id="e1db7-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1db7-142">请求</span><span class="sxs-lookup"><span data-stu-id="e1db7-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e1db7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1db7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="e1db7-144">C#</span><span class="sxs-lookup"><span data-stu-id="e1db7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1db7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1db7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1db7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1db7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1db7-147">Java</span><span class="sxs-lookup"><span data-stu-id="e1db7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e1db7-148">响应</span><span class="sxs-lookup"><span data-stu-id="e1db7-148">Response</span></span>
<span data-ttu-id="e1db7-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e1db7-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

