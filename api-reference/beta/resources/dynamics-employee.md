---
title: 员工资源类型
description: Dynamics 365 Business Central 中的 employee 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543061"
---
# <a name="employees-resource-type"></a><span data-ttu-id="24d5e-103">员工资源类型</span><span class="sxs-lookup"><span data-stu-id="24d5e-103">employees resource type</span></span>
<span data-ttu-id="24d5e-104">表示 Dynamics 365 Business Central 中的员工。</span><span class="sxs-lookup"><span data-stu-id="24d5e-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="24d5e-105">方法</span><span class="sxs-lookup"><span data-stu-id="24d5e-105">Methods</span></span>

| <span data-ttu-id="24d5e-106">方法</span><span class="sxs-lookup"><span data-stu-id="24d5e-106">Method</span></span>                                              | <span data-ttu-id="24d5e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="24d5e-107">Return Type</span></span>|<span data-ttu-id="24d5e-108">说明</span><span class="sxs-lookup"><span data-stu-id="24d5e-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="24d5e-109">获取员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="24d5e-110">员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-110">employees</span></span>  |<span data-ttu-id="24d5e-111">获取一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="24d5e-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="24d5e-112">过帐员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="24d5e-113">员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-113">employees</span></span>  |<span data-ttu-id="24d5e-114">创建一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="24d5e-114">Create an employee object.</span></span>|
|[<span data-ttu-id="24d5e-115">修补员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="24d5e-116">员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-116">employees</span></span>  |<span data-ttu-id="24d5e-117">更新 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="24d5e-117">Update an employee object.</span></span>|
|[<span data-ttu-id="24d5e-118">删除员工</span><span class="sxs-lookup"><span data-stu-id="24d5e-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="24d5e-119">无</span><span class="sxs-lookup"><span data-stu-id="24d5e-119">none</span></span>       |<span data-ttu-id="24d5e-120">删除 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="24d5e-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="24d5e-121">属性</span><span class="sxs-lookup"><span data-stu-id="24d5e-121">Properties</span></span>
| <span data-ttu-id="24d5e-122">属性</span><span class="sxs-lookup"><span data-stu-id="24d5e-122">Property</span></span>           | <span data-ttu-id="24d5e-123">类型</span><span class="sxs-lookup"><span data-stu-id="24d5e-123">Type</span></span>   |<span data-ttu-id="24d5e-124">说明</span><span class="sxs-lookup"><span data-stu-id="24d5e-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="24d5e-125">id</span><span class="sxs-lookup"><span data-stu-id="24d5e-125">id</span></span>                  |<span data-ttu-id="24d5e-126">GUID</span><span class="sxs-lookup"><span data-stu-id="24d5e-126">GUID</span></span>    |<span data-ttu-id="24d5e-127">员工 ID。</span><span class="sxs-lookup"><span data-stu-id="24d5e-127">The employee ID.</span></span> <span data-ttu-id="24d5e-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="24d5e-128">Non-editable.</span></span>                         |
|<span data-ttu-id="24d5e-129">数字</span><span class="sxs-lookup"><span data-stu-id="24d5e-129">number</span></span>              |<span data-ttu-id="24d5e-130">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-130">string</span></span>  |<span data-ttu-id="24d5e-131">员工编号。</span><span class="sxs-lookup"><span data-stu-id="24d5e-131">The employee number.</span></span> <span data-ttu-id="24d5e-132">只读。</span><span class="sxs-lookup"><span data-stu-id="24d5e-132">Read-Only.</span></span>                        |
|<span data-ttu-id="24d5e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="24d5e-133">displayName</span></span>         |<span data-ttu-id="24d5e-134">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-134">string</span></span>  |<span data-ttu-id="24d5e-135">员工 givenName + 姓。</span><span class="sxs-lookup"><span data-stu-id="24d5e-135">The employee givenName + surname.</span></span> <span data-ttu-id="24d5e-136">只读。</span><span class="sxs-lookup"><span data-stu-id="24d5e-136">Read-Only.</span></span>           |
|<span data-ttu-id="24d5e-137">givenName</span><span class="sxs-lookup"><span data-stu-id="24d5e-137">givenName</span></span>           |<span data-ttu-id="24d5e-138">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-138">string</span></span>  |<span data-ttu-id="24d5e-139">员工的名字。</span><span class="sxs-lookup"><span data-stu-id="24d5e-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="24d5e-140">middleName</span><span class="sxs-lookup"><span data-stu-id="24d5e-140">middleName</span></span>          |<span data-ttu-id="24d5e-141">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-141">string</span></span>  |<span data-ttu-id="24d5e-142">员工的中间名。</span><span class="sxs-lookup"><span data-stu-id="24d5e-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="24d5e-143">surname</span><span class="sxs-lookup"><span data-stu-id="24d5e-143">surname</span></span>             |<span data-ttu-id="24d5e-144">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-144">string</span></span>  |<span data-ttu-id="24d5e-145">员工的姓氏</span><span class="sxs-lookup"><span data-stu-id="24d5e-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="24d5e-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="24d5e-146">jobTitle</span></span>            |<span data-ttu-id="24d5e-147">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-147">string</span></span>  |<span data-ttu-id="24d5e-148">员工的完整名称</span><span class="sxs-lookup"><span data-stu-id="24d5e-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="24d5e-149">address</span><span class="sxs-lookup"><span data-stu-id="24d5e-149">address</span></span>             |[<span data-ttu-id="24d5e-150">翻.省略</span><span class="sxs-lookup"><span data-stu-id="24d5e-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="24d5e-151">指定员工的地址。</span><span class="sxs-lookup"><span data-stu-id="24d5e-151">Specifies the employee's address.</span></span> <span data-ttu-id="24d5e-152">此地址将显示在员工的所有资源文档中。</span><span class="sxs-lookup"><span data-stu-id="24d5e-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="24d5e-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="24d5e-153">phoneNumber</span></span>         |<span data-ttu-id="24d5e-154">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-154">string</span></span>  |<span data-ttu-id="24d5e-155">指定员工的电话号码。</span><span class="sxs-lookup"><span data-stu-id="24d5e-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="24d5e-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="24d5e-156">mobilePhone</span></span>         |<span data-ttu-id="24d5e-157">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-157">string</span></span>  |<span data-ttu-id="24d5e-158">指定员工的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="24d5e-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="24d5e-159">email</span><span class="sxs-lookup"><span data-stu-id="24d5e-159">email</span></span>               |<span data-ttu-id="24d5e-160">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-160">string</span></span>  |<span data-ttu-id="24d5e-161">指定员工的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="24d5e-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="24d5e-162">personalEmail</span><span class="sxs-lookup"><span data-stu-id="24d5e-162">personalEmail</span></span>       |<span data-ttu-id="24d5e-163">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-163">string</span></span>  |<span data-ttu-id="24d5e-164">指定员工的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="24d5e-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="24d5e-165">employmentDate</span><span class="sxs-lookup"><span data-stu-id="24d5e-165">employmentDate</span></span>      |<span data-ttu-id="24d5e-166">date</span><span class="sxs-lookup"><span data-stu-id="24d5e-166">date</span></span>    |<span data-ttu-id="24d5e-167">指定员工开始为公司工作的日期。</span><span class="sxs-lookup"><span data-stu-id="24d5e-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="24d5e-168">terminationDate</span><span class="sxs-lookup"><span data-stu-id="24d5e-168">terminationDate</span></span>     |<span data-ttu-id="24d5e-169">date</span><span class="sxs-lookup"><span data-stu-id="24d5e-169">date</span></span>    |<span data-ttu-id="24d5e-170">指定由于退休或开除而终止员工的日期。</span><span class="sxs-lookup"><span data-stu-id="24d5e-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="24d5e-171">status</span><span class="sxs-lookup"><span data-stu-id="24d5e-171">status</span></span>              |<span data-ttu-id="24d5e-172">string</span><span class="sxs-lookup"><span data-stu-id="24d5e-172">string</span></span>  |<span data-ttu-id="24d5e-173">指定员工的状态。</span><span class="sxs-lookup"><span data-stu-id="24d5e-173">Specifies the employee's status.</span></span> <span data-ttu-id="24d5e-174">可能的值包括活动、非活动或已终止</span><span class="sxs-lookup"><span data-stu-id="24d5e-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="24d5e-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="24d5e-175">birthDate</span></span>           |<span data-ttu-id="24d5e-176">date</span><span class="sxs-lookup"><span data-stu-id="24d5e-176">date</span></span>    |<span data-ttu-id="24d5e-177">指定员工的出生日期。</span><span class="sxs-lookup"><span data-stu-id="24d5e-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="24d5e-178">头像</span><span class="sxs-lookup"><span data-stu-id="24d5e-178">picture</span></span>             |<span data-ttu-id="24d5e-179">stream</span><span class="sxs-lookup"><span data-stu-id="24d5e-179">stream</span></span>  |<span data-ttu-id="24d5e-180">员工头像。</span><span class="sxs-lookup"><span data-stu-id="24d5e-180">The employee picture.</span></span> <span data-ttu-id="24d5e-181">只读。</span><span class="sxs-lookup"><span data-stu-id="24d5e-181">Read-Only.</span></span>                       |
|<span data-ttu-id="24d5e-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24d5e-182">lastModifiedDateTime</span></span>|<span data-ttu-id="24d5e-183">datetime</span><span class="sxs-lookup"><span data-stu-id="24d5e-183">datetime</span></span>|<span data-ttu-id="24d5e-184">上次修改员工的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24d5e-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="24d5e-185">只读。</span><span class="sxs-lookup"><span data-stu-id="24d5e-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="24d5e-186">关系</span><span class="sxs-lookup"><span data-stu-id="24d5e-186">Relationships</span></span>
<span data-ttu-id="24d5e-187">无</span><span class="sxs-lookup"><span data-stu-id="24d5e-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24d5e-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24d5e-188">JSON representation</span></span>

<span data-ttu-id="24d5e-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24d5e-189">Here is a JSON representation of the resource.</span></span>


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

