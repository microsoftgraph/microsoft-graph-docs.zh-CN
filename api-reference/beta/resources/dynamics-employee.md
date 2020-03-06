---
title: 员工资源类型
description: Dynamics 365 Business Central 中的 employee 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 84fccbcb9d60c97a2ce0079a9ba773a8400a8069
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504081"
---
# <a name="employees-resource-type"></a><span data-ttu-id="1495a-103">员工资源类型</span><span class="sxs-lookup"><span data-stu-id="1495a-103">employees resource type</span></span>

<span data-ttu-id="1495a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1495a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1495a-105">表示 Dynamics 365 Business Central 中的员工。</span><span class="sxs-lookup"><span data-stu-id="1495a-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1495a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1495a-106">Methods</span></span>

| <span data-ttu-id="1495a-107">方法</span><span class="sxs-lookup"><span data-stu-id="1495a-107">Method</span></span>                                              | <span data-ttu-id="1495a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1495a-108">Return Type</span></span>|<span data-ttu-id="1495a-109">说明</span><span class="sxs-lookup"><span data-stu-id="1495a-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="1495a-110">获取员工</span><span class="sxs-lookup"><span data-stu-id="1495a-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="1495a-111">员工</span><span class="sxs-lookup"><span data-stu-id="1495a-111">employees</span></span>  |<span data-ttu-id="1495a-112">获取一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="1495a-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="1495a-113">过帐员工</span><span class="sxs-lookup"><span data-stu-id="1495a-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="1495a-114">员工</span><span class="sxs-lookup"><span data-stu-id="1495a-114">employees</span></span>  |<span data-ttu-id="1495a-115">创建一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="1495a-115">Create an employee object.</span></span>|
|[<span data-ttu-id="1495a-116">修补员工</span><span class="sxs-lookup"><span data-stu-id="1495a-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="1495a-117">员工</span><span class="sxs-lookup"><span data-stu-id="1495a-117">employees</span></span>  |<span data-ttu-id="1495a-118">更新 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="1495a-118">Update an employee object.</span></span>|
|[<span data-ttu-id="1495a-119">删除员工</span><span class="sxs-lookup"><span data-stu-id="1495a-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="1495a-120">无</span><span class="sxs-lookup"><span data-stu-id="1495a-120">none</span></span>       |<span data-ttu-id="1495a-121">删除 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="1495a-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1495a-122">属性</span><span class="sxs-lookup"><span data-stu-id="1495a-122">Properties</span></span>
| <span data-ttu-id="1495a-123">属性</span><span class="sxs-lookup"><span data-stu-id="1495a-123">Property</span></span>           | <span data-ttu-id="1495a-124">类型</span><span class="sxs-lookup"><span data-stu-id="1495a-124">Type</span></span>   |<span data-ttu-id="1495a-125">说明</span><span class="sxs-lookup"><span data-stu-id="1495a-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="1495a-126">id</span><span class="sxs-lookup"><span data-stu-id="1495a-126">id</span></span>                  |<span data-ttu-id="1495a-127">GUID</span><span class="sxs-lookup"><span data-stu-id="1495a-127">GUID</span></span>    |<span data-ttu-id="1495a-128">员工 ID。</span><span class="sxs-lookup"><span data-stu-id="1495a-128">The employee ID.</span></span> <span data-ttu-id="1495a-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="1495a-129">Non-editable.</span></span>                         |
|<span data-ttu-id="1495a-130">number</span><span class="sxs-lookup"><span data-stu-id="1495a-130">number</span></span>              |<span data-ttu-id="1495a-131">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-131">string</span></span>  |<span data-ttu-id="1495a-132">员工编号。</span><span class="sxs-lookup"><span data-stu-id="1495a-132">The employee number.</span></span> <span data-ttu-id="1495a-133">只读。</span><span class="sxs-lookup"><span data-stu-id="1495a-133">Read-Only.</span></span>                        |
|<span data-ttu-id="1495a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1495a-134">displayName</span></span>         |<span data-ttu-id="1495a-135">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-135">string</span></span>  |<span data-ttu-id="1495a-136">员工 givenName + 姓。</span><span class="sxs-lookup"><span data-stu-id="1495a-136">The employee givenName + surname.</span></span> <span data-ttu-id="1495a-137">只读。</span><span class="sxs-lookup"><span data-stu-id="1495a-137">Read-Only.</span></span>           |
|<span data-ttu-id="1495a-138">givenName</span><span class="sxs-lookup"><span data-stu-id="1495a-138">givenName</span></span>           |<span data-ttu-id="1495a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-139">string</span></span>  |<span data-ttu-id="1495a-140">员工的名字。</span><span class="sxs-lookup"><span data-stu-id="1495a-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="1495a-141">middleName</span><span class="sxs-lookup"><span data-stu-id="1495a-141">middleName</span></span>          |<span data-ttu-id="1495a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-142">string</span></span>  |<span data-ttu-id="1495a-143">员工的中间名。</span><span class="sxs-lookup"><span data-stu-id="1495a-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="1495a-144">surname</span><span class="sxs-lookup"><span data-stu-id="1495a-144">surname</span></span>             |<span data-ttu-id="1495a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-145">string</span></span>  |<span data-ttu-id="1495a-146">员工的姓氏</span><span class="sxs-lookup"><span data-stu-id="1495a-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="1495a-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="1495a-147">jobTitle</span></span>            |<span data-ttu-id="1495a-148">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-148">string</span></span>  |<span data-ttu-id="1495a-149">员工的完整名称</span><span class="sxs-lookup"><span data-stu-id="1495a-149">The full name of the employee</span></span>                          |
|<span data-ttu-id="1495a-150">address</span><span class="sxs-lookup"><span data-stu-id="1495a-150">address</span></span>             |[<span data-ttu-id="1495a-151">翻.省略</span><span class="sxs-lookup"><span data-stu-id="1495a-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="1495a-152">指定员工的地址。</span><span class="sxs-lookup"><span data-stu-id="1495a-152">Specifies the employee's address.</span></span> <span data-ttu-id="1495a-153">此地址将显示在员工的所有资源文档中。</span><span class="sxs-lookup"><span data-stu-id="1495a-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="1495a-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1495a-154">phoneNumber</span></span>         |<span data-ttu-id="1495a-155">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-155">string</span></span>  |<span data-ttu-id="1495a-156">指定员工的电话号码。</span><span class="sxs-lookup"><span data-stu-id="1495a-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="1495a-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="1495a-157">mobilePhone</span></span>         |<span data-ttu-id="1495a-158">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-158">string</span></span>  |<span data-ttu-id="1495a-159">指定员工的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="1495a-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="1495a-160">email</span><span class="sxs-lookup"><span data-stu-id="1495a-160">email</span></span>               |<span data-ttu-id="1495a-161">string</span><span class="sxs-lookup"><span data-stu-id="1495a-161">string</span></span>  |<span data-ttu-id="1495a-162">指定员工的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1495a-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="1495a-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="1495a-163">personalEmail</span></span>       |<span data-ttu-id="1495a-164">字符串</span><span class="sxs-lookup"><span data-stu-id="1495a-164">string</span></span>  |<span data-ttu-id="1495a-165">指定员工的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1495a-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="1495a-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="1495a-166">employmentDate</span></span>      |<span data-ttu-id="1495a-167">date</span><span class="sxs-lookup"><span data-stu-id="1495a-167">date</span></span>    |<span data-ttu-id="1495a-168">指定员工开始为公司工作的日期。</span><span class="sxs-lookup"><span data-stu-id="1495a-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="1495a-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="1495a-169">terminationDate</span></span>     |<span data-ttu-id="1495a-170">date</span><span class="sxs-lookup"><span data-stu-id="1495a-170">date</span></span>    |<span data-ttu-id="1495a-171">指定由于退休或开除而终止员工的日期。</span><span class="sxs-lookup"><span data-stu-id="1495a-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="1495a-172">状态</span><span class="sxs-lookup"><span data-stu-id="1495a-172">status</span></span>              |<span data-ttu-id="1495a-173">string</span><span class="sxs-lookup"><span data-stu-id="1495a-173">string</span></span>  |<span data-ttu-id="1495a-174">指定员工的状态。</span><span class="sxs-lookup"><span data-stu-id="1495a-174">Specifies the employee's status.</span></span> <span data-ttu-id="1495a-175">可能的值包括活动、非活动或已终止</span><span class="sxs-lookup"><span data-stu-id="1495a-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="1495a-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="1495a-176">birthDate</span></span>           |<span data-ttu-id="1495a-177">date</span><span class="sxs-lookup"><span data-stu-id="1495a-177">date</span></span>    |<span data-ttu-id="1495a-178">指定员工的出生日期。</span><span class="sxs-lookup"><span data-stu-id="1495a-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="1495a-179">头像</span><span class="sxs-lookup"><span data-stu-id="1495a-179">picture</span></span>             |<span data-ttu-id="1495a-180">stream</span><span class="sxs-lookup"><span data-stu-id="1495a-180">stream</span></span>  |<span data-ttu-id="1495a-181">员工头像。</span><span class="sxs-lookup"><span data-stu-id="1495a-181">The employee picture.</span></span> <span data-ttu-id="1495a-182">只读。</span><span class="sxs-lookup"><span data-stu-id="1495a-182">Read-Only.</span></span>                       |
|<span data-ttu-id="1495a-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1495a-183">lastModifiedDateTime</span></span>|<span data-ttu-id="1495a-184">datetime</span><span class="sxs-lookup"><span data-stu-id="1495a-184">datetime</span></span>|<span data-ttu-id="1495a-185">上次修改员工的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1495a-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="1495a-186">只读。</span><span class="sxs-lookup"><span data-stu-id="1495a-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="1495a-187">关系</span><span class="sxs-lookup"><span data-stu-id="1495a-187">Relationships</span></span>
<span data-ttu-id="1495a-188">无</span><span class="sxs-lookup"><span data-stu-id="1495a-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1495a-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1495a-189">JSON representation</span></span>

<span data-ttu-id="1495a-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1495a-190">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

