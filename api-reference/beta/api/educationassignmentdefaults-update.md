---
title: 更新 educationAssignmentDefaults
description: 更新 educationAssignmentDefaults 对象的属性。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 13a7b9b387581612193e4759521daa42216b2be0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470314"
---
# <a name="update-educationassignmentdefaults"></a><span data-ttu-id="a5c85-103">更新 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="a5c85-103">Update educationAssignmentDefaults</span></span>
<span data-ttu-id="a5c85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5c85-105">更新 [educationAssignmentDefaults 对象](../resources/educationassignmentdefaults.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a5c85-105">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> <span data-ttu-id="a5c85-106">只有教师可以更新这些设置。</span><span class="sxs-lookup"><span data-stu-id="a5c85-106">Only teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5c85-107">权限</span><span class="sxs-lookup"><span data-stu-id="a5c85-107">Permissions</span></span>
<span data-ttu-id="a5c85-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5c85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c85-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5c85-110">Permission type</span></span>|<span data-ttu-id="a5c85-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5c85-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5c85-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5c85-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5c85-113">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5c85-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a5c85-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5c85-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a5c85-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5c85-115">Not supported.</span></span>  |
|<span data-ttu-id="a5c85-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5c85-116">Application</span></span> | <span data-ttu-id="a5c85-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5c85-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5c85-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5c85-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentDefaults
```

## <a name="request-headers"></a><span data-ttu-id="a5c85-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5c85-119">Request headers</span></span>
|<span data-ttu-id="a5c85-120">名称</span><span class="sxs-lookup"><span data-stu-id="a5c85-120">Name</span></span>|<span data-ttu-id="a5c85-121">说明</span><span class="sxs-lookup"><span data-stu-id="a5c85-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5c85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5c85-122">Authorization</span></span>|<span data-ttu-id="a5c85-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5c85-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a5c85-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5c85-125">Content-Type</span></span>|<span data-ttu-id="a5c85-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a5c85-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5c85-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5c85-128">Request body</span></span>
<span data-ttu-id="a5c85-129">在请求正文中，提供 [应更新的 educationAssignmentDefaults](../resources/educationassignmentdefaults.md) 对象的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a5c85-129">In the request body, supply the values for relevant fields of the [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object that should be updated.</span></span> <span data-ttu-id="a5c85-130">请求正文中不包含的现有属性将保留其以前的值。</span><span class="sxs-lookup"><span data-stu-id="a5c85-130">Existing properties that are not included in the request body will maintain their previous values.</span></span> <span data-ttu-id="a5c85-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a5c85-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="a5c85-132">属性</span><span class="sxs-lookup"><span data-stu-id="a5c85-132">Property</span></span>|<span data-ttu-id="a5c85-133">类型</span><span class="sxs-lookup"><span data-stu-id="a5c85-133">Type</span></span>|<span data-ttu-id="a5c85-134">说明</span><span class="sxs-lookup"><span data-stu-id="a5c85-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c85-135">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="a5c85-135">addedStudentAction</span></span>|<span data-ttu-id="a5c85-136">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="a5c85-136">educationAddedStudentAction</span></span>|<span data-ttu-id="a5c85-137">用于处理作业发布后添加的学生的课堂级别默认行为。</span><span class="sxs-lookup"><span data-stu-id="a5c85-137">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="a5c85-138">可取值为：`none`、`assignIfOpen`。</span><span class="sxs-lookup"><span data-stu-id="a5c85-138">Possible values are: `none`, `assignIfOpen`.</span></span> <span data-ttu-id="a5c85-139">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="a5c85-139">The default value is `none`.</span></span>|
|<span data-ttu-id="a5c85-140">dueTime</span><span class="sxs-lookup"><span data-stu-id="a5c85-140">dueTime</span></span>|<span data-ttu-id="a5c85-141">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a5c85-141">TimeOfDay</span></span>|<span data-ttu-id="a5c85-142">截止日期域的类级别默认值。</span><span class="sxs-lookup"><span data-stu-id="a5c85-142">Class-level default value for due time field.</span></span> <span data-ttu-id="a5c85-143">默认值为 `23:59:00`</span><span class="sxs-lookup"><span data-stu-id="a5c85-143">Default value is `23:59:00`</span></span>|
|<span data-ttu-id="a5c85-144">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="a5c85-144">notificationChannelUrl</span></span>|<span data-ttu-id="a5c85-145">String</span><span class="sxs-lookup"><span data-stu-id="a5c85-145">String</span></span>|<span data-ttu-id="a5c85-146">通知将发送到的默认 Teams 频道。</span><span class="sxs-lookup"><span data-stu-id="a5c85-146">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="a5c85-147">默认值为 `null`。</span><span class="sxs-lookup"><span data-stu-id="a5c85-147">Default value is `null`.</span></span>|



## <a name="response"></a><span data-ttu-id="a5c85-148">响应</span><span class="sxs-lookup"><span data-stu-id="a5c85-148">Response</span></span>

<span data-ttu-id="a5c85-149">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 educationAssignmentDefaults](../resources/educationassignmentdefaults.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a5c85-149">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5c85-150">示例</span><span class="sxs-lookup"><span data-stu-id="a5c85-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5c85-151">请求</span><span class="sxs-lookup"><span data-stu-id="a5c85-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a5c85-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c85-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```
# <a name="c"></a>[<span data-ttu-id="a5c85-153">C#</span><span class="sxs-lookup"><span data-stu-id="a5c85-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5c85-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c85-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5c85-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5c85-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5c85-156">Java</span><span class="sxs-lookup"><span data-stu-id="a5c85-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a5c85-157">响应</span><span class="sxs-lookup"><span data-stu-id="a5c85-157">Response</span></span>
<span data-ttu-id="a5c85-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a5c85-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "addedStudentAction": "assignIfOpen",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

