---
title: 员工资源类型
description: Dynamics 365 Business Central 中的 employee 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 96d44856ad52c983e61181fc64b93477fbe79e6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972948"
---
# <a name="employees-resource-type"></a><span data-ttu-id="b1a3d-103">员工资源类型</span><span class="sxs-lookup"><span data-stu-id="b1a3d-103">employees resource type</span></span>
<span data-ttu-id="b1a3d-104">表示 Dynamics 365 Business Central 中的员工。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b1a3d-105">方法</span><span class="sxs-lookup"><span data-stu-id="b1a3d-105">Methods</span></span>

| <span data-ttu-id="b1a3d-106">方法</span><span class="sxs-lookup"><span data-stu-id="b1a3d-106">Method</span></span>                                              | <span data-ttu-id="b1a3d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1a3d-107">Return Type</span></span>|<span data-ttu-id="b1a3d-108">说明</span><span class="sxs-lookup"><span data-stu-id="b1a3d-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="b1a3d-109">获取员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="b1a3d-110">员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-110">employees</span></span>  |<span data-ttu-id="b1a3d-111">获取一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="b1a3d-112">过帐员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="b1a3d-113">员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-113">employees</span></span>  |<span data-ttu-id="b1a3d-114">创建一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-114">Create an employee object.</span></span>|
|[<span data-ttu-id="b1a3d-115">修补员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="b1a3d-116">员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-116">employees</span></span>  |<span data-ttu-id="b1a3d-117">更新 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-117">Update an employee object.</span></span>|
|[<span data-ttu-id="b1a3d-118">删除员工</span><span class="sxs-lookup"><span data-stu-id="b1a3d-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="b1a3d-119">无</span><span class="sxs-lookup"><span data-stu-id="b1a3d-119">none</span></span>       |<span data-ttu-id="b1a3d-120">删除 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1a3d-121">属性</span><span class="sxs-lookup"><span data-stu-id="b1a3d-121">Properties</span></span>
| <span data-ttu-id="b1a3d-122">属性</span><span class="sxs-lookup"><span data-stu-id="b1a3d-122">Property</span></span>           | <span data-ttu-id="b1a3d-123">类型</span><span class="sxs-lookup"><span data-stu-id="b1a3d-123">Type</span></span>   |<span data-ttu-id="b1a3d-124">说明</span><span class="sxs-lookup"><span data-stu-id="b1a3d-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="b1a3d-125">id</span><span class="sxs-lookup"><span data-stu-id="b1a3d-125">id</span></span>                  |<span data-ttu-id="b1a3d-126">GUID</span><span class="sxs-lookup"><span data-stu-id="b1a3d-126">GUID</span></span>    |<span data-ttu-id="b1a3d-127">员工 ID。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-127">The employee ID.</span></span> <span data-ttu-id="b1a3d-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-128">Non-editable.</span></span>                         |
|<span data-ttu-id="b1a3d-129">number</span><span class="sxs-lookup"><span data-stu-id="b1a3d-129">number</span></span>              |<span data-ttu-id="b1a3d-130">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-130">string</span></span>  |<span data-ttu-id="b1a3d-131">员工编号。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-131">The employee number.</span></span> <span data-ttu-id="b1a3d-132">只读。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-132">Read-Only.</span></span>                        |
|<span data-ttu-id="b1a3d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b1a3d-133">displayName</span></span>         |<span data-ttu-id="b1a3d-134">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-134">string</span></span>  |<span data-ttu-id="b1a3d-135">员工 givenName + 姓。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-135">The employee givenName + surname.</span></span> <span data-ttu-id="b1a3d-136">只读。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-136">Read-Only.</span></span>           |
|<span data-ttu-id="b1a3d-137">givenName</span><span class="sxs-lookup"><span data-stu-id="b1a3d-137">givenName</span></span>           |<span data-ttu-id="b1a3d-138">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-138">string</span></span>  |<span data-ttu-id="b1a3d-139">员工的名字。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="b1a3d-140">middleName</span><span class="sxs-lookup"><span data-stu-id="b1a3d-140">middleName</span></span>          |<span data-ttu-id="b1a3d-141">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-141">string</span></span>  |<span data-ttu-id="b1a3d-142">员工的中间名。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="b1a3d-143">surname</span><span class="sxs-lookup"><span data-stu-id="b1a3d-143">surname</span></span>             |<span data-ttu-id="b1a3d-144">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-144">string</span></span>  |<span data-ttu-id="b1a3d-145">员工的姓氏</span><span class="sxs-lookup"><span data-stu-id="b1a3d-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="b1a3d-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b1a3d-146">jobTitle</span></span>            |<span data-ttu-id="b1a3d-147">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-147">string</span></span>  |<span data-ttu-id="b1a3d-148">员工的完整名称</span><span class="sxs-lookup"><span data-stu-id="b1a3d-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="b1a3d-149">address</span><span class="sxs-lookup"><span data-stu-id="b1a3d-149">address</span></span>             |[<span data-ttu-id="b1a3d-150">翻.省略</span><span class="sxs-lookup"><span data-stu-id="b1a3d-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="b1a3d-151">指定员工的地址。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-151">Specifies the employee's address.</span></span> <span data-ttu-id="b1a3d-152">此地址将显示在员工的所有资源文档中。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="b1a3d-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b1a3d-153">phoneNumber</span></span>         |<span data-ttu-id="b1a3d-154">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-154">string</span></span>  |<span data-ttu-id="b1a3d-155">指定员工的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="b1a3d-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b1a3d-156">mobilePhone</span></span>         |<span data-ttu-id="b1a3d-157">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-157">string</span></span>  |<span data-ttu-id="b1a3d-158">指定员工的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="b1a3d-159">email</span><span class="sxs-lookup"><span data-stu-id="b1a3d-159">email</span></span>               |<span data-ttu-id="b1a3d-160">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-160">string</span></span>  |<span data-ttu-id="b1a3d-161">指定员工的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="b1a3d-162">personalEmail</span><span class="sxs-lookup"><span data-stu-id="b1a3d-162">personalEmail</span></span>       |<span data-ttu-id="b1a3d-163">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-163">string</span></span>  |<span data-ttu-id="b1a3d-164">指定员工的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="b1a3d-165">employmentDate</span><span class="sxs-lookup"><span data-stu-id="b1a3d-165">employmentDate</span></span>      |<span data-ttu-id="b1a3d-166">date</span><span class="sxs-lookup"><span data-stu-id="b1a3d-166">date</span></span>    |<span data-ttu-id="b1a3d-167">指定员工开始为公司工作的日期。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="b1a3d-168">terminationDate</span><span class="sxs-lookup"><span data-stu-id="b1a3d-168">terminationDate</span></span>     |<span data-ttu-id="b1a3d-169">date</span><span class="sxs-lookup"><span data-stu-id="b1a3d-169">date</span></span>    |<span data-ttu-id="b1a3d-170">指定由于退休或开除而终止员工的日期。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="b1a3d-171">状态</span><span class="sxs-lookup"><span data-stu-id="b1a3d-171">status</span></span>              |<span data-ttu-id="b1a3d-172">string</span><span class="sxs-lookup"><span data-stu-id="b1a3d-172">string</span></span>  |<span data-ttu-id="b1a3d-173">指定员工的状态。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-173">Specifies the employee's status.</span></span> <span data-ttu-id="b1a3d-174">可能的值包括活动、非活动或已终止</span><span class="sxs-lookup"><span data-stu-id="b1a3d-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="b1a3d-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="b1a3d-175">birthDate</span></span>           |<span data-ttu-id="b1a3d-176">date</span><span class="sxs-lookup"><span data-stu-id="b1a3d-176">date</span></span>    |<span data-ttu-id="b1a3d-177">指定员工的出生日期。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="b1a3d-178">头像</span><span class="sxs-lookup"><span data-stu-id="b1a3d-178">picture</span></span>             |<span data-ttu-id="b1a3d-179">stream</span><span class="sxs-lookup"><span data-stu-id="b1a3d-179">stream</span></span>  |<span data-ttu-id="b1a3d-180">员工头像。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-180">The employee picture.</span></span> <span data-ttu-id="b1a3d-181">只读。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-181">Read-Only.</span></span>                       |
|<span data-ttu-id="b1a3d-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1a3d-182">lastModifiedDateTime</span></span>|<span data-ttu-id="b1a3d-183">datetime</span><span class="sxs-lookup"><span data-stu-id="b1a3d-183">datetime</span></span>|<span data-ttu-id="b1a3d-184">上次修改员工的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="b1a3d-185">只读。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="b1a3d-186">关系</span><span class="sxs-lookup"><span data-stu-id="b1a3d-186">Relationships</span></span>
<span data-ttu-id="b1a3d-187">无</span><span class="sxs-lookup"><span data-stu-id="b1a3d-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1a3d-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1a3d-188">JSON representation</span></span>

<span data-ttu-id="b1a3d-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1a3d-189">Here is a JSON representation of the resource.</span></span>


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

