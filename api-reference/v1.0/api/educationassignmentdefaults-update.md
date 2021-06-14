---
title: 更新 educationAssignmentDefaults
description: 更新 educationAssignmentDefaults 对象的属性。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7f73af01d485bfade10dfae769290eb40a36c656
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911397"
---
# <a name="update-educationassignmentdefaults"></a><span data-ttu-id="d0777-103">更新 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="d0777-103">Update educationAssignmentDefaults</span></span>
<span data-ttu-id="d0777-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0777-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0777-105">更新 [educationAssignmentDefaults 对象](../resources/educationassignmentdefaults.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d0777-105">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>

<span data-ttu-id="d0777-106">只有教师可以更新这些设置。</span><span class="sxs-lookup"><span data-stu-id="d0777-106">Only teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0777-107">权限</span><span class="sxs-lookup"><span data-stu-id="d0777-107">Permissions</span></span>
<span data-ttu-id="d0777-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0777-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0777-110">Permission type</span></span>|<span data-ttu-id="d0777-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0777-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0777-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0777-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d0777-113">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0777-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d0777-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0777-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0777-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0777-115">Not supported.</span></span>  |
|<span data-ttu-id="d0777-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0777-116">Application</span></span> | <span data-ttu-id="d0777-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0777-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0777-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0777-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

## <a name="request-headers"></a><span data-ttu-id="d0777-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0777-119">Request headers</span></span>
|<span data-ttu-id="d0777-120">名称</span><span class="sxs-lookup"><span data-stu-id="d0777-120">Name</span></span>|<span data-ttu-id="d0777-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0777-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0777-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0777-122">Authorization</span></span>|<span data-ttu-id="d0777-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0777-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0777-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0777-125">Content-Type</span></span>|<span data-ttu-id="d0777-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d0777-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0777-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0777-128">Request body</span></span>
<span data-ttu-id="d0777-129">在请求正文中，仅提供要更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="d0777-129">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="d0777-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d0777-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0777-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d0777-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d0777-132">属性</span><span class="sxs-lookup"><span data-stu-id="d0777-132">Property</span></span>|<span data-ttu-id="d0777-133">类型</span><span class="sxs-lookup"><span data-stu-id="d0777-133">Type</span></span>|<span data-ttu-id="d0777-134">说明</span><span class="sxs-lookup"><span data-stu-id="d0777-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0777-135">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d0777-135">addedStudentAction</span></span>|<span data-ttu-id="d0777-136">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d0777-136">educationAddedStudentAction</span></span>| <span data-ttu-id="d0777-137">在作业发布日期之后添加的学生的课堂级别默认操作。</span><span class="sxs-lookup"><span data-stu-id="d0777-137">Class-level default actions for students added after the assignment publication date.</span></span> <span data-ttu-id="d0777-138">可取值为：`none`、`assignIfOpen`。</span><span class="sxs-lookup"><span data-stu-id="d0777-138">Possible values are: `none`, `assignIfOpen`.</span></span> <span data-ttu-id="d0777-139">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="d0777-139">The default value is `none`.</span></span>|
|<span data-ttu-id="d0777-140">dueTime</span><span class="sxs-lookup"><span data-stu-id="d0777-140">dueTime</span></span>|<span data-ttu-id="d0777-141">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d0777-141">TimeOfDay</span></span>| <span data-ttu-id="d0777-142">"到期时间"字段的类级别默认值。</span><span class="sxs-lookup"><span data-stu-id="d0777-142">Class-level default value for due time field.</span></span> <span data-ttu-id="d0777-143">默认值为 `23:59:00`</span><span class="sxs-lookup"><span data-stu-id="d0777-143">Default value is `23:59:00`</span></span>|
|<span data-ttu-id="d0777-144">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="d0777-144">notificationChannelUrl</span></span>|<span data-ttu-id="d0777-145">String</span><span class="sxs-lookup"><span data-stu-id="d0777-145">String</span></span>| <span data-ttu-id="d0777-146">默认Teams发送与分配相关的通知的通道。</span><span class="sxs-lookup"><span data-stu-id="d0777-146">Default Teams channel to send notifications related to the assignment.</span></span> <span data-ttu-id="d0777-147">默认值为 `null`。</span><span class="sxs-lookup"><span data-stu-id="d0777-147">Default value is `null`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0777-148">响应</span><span class="sxs-lookup"><span data-stu-id="d0777-148">Response</span></span>

<span data-ttu-id="d0777-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0777-149">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0777-150">示例</span><span class="sxs-lookup"><span data-stu-id="d0777-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0777-151">请求</span><span class="sxs-lookup"><span data-stu-id="d0777-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}
```

### <a name="response"></a><span data-ttu-id="d0777-152">响应</span><span class="sxs-lookup"><span data-stu-id="d0777-152">Response</span></span>
<span data-ttu-id="d0777-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0777-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "dueTime": "String",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}
```

