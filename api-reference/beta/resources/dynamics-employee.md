---
title: employees 资源类型
description: Dynamics 365 Business Central 中的员工对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: eceea9e1811b61045c03fb8dc5d7710f33158ccc
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695971"
---
# <a name="employees-resource-type"></a><span data-ttu-id="448d3-103">employees 资源类型</span><span class="sxs-lookup"><span data-stu-id="448d3-103">employees resource type</span></span>

<span data-ttu-id="448d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="448d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="448d3-105">表示 Dynamics 365 Business Central 中的员工。</span><span class="sxs-lookup"><span data-stu-id="448d3-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="448d3-106">方法</span><span class="sxs-lookup"><span data-stu-id="448d3-106">Methods</span></span>

| <span data-ttu-id="448d3-107">方法</span><span class="sxs-lookup"><span data-stu-id="448d3-107">Method</span></span>                                              | <span data-ttu-id="448d3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="448d3-108">Return Type</span></span>|<span data-ttu-id="448d3-109">说明</span><span class="sxs-lookup"><span data-stu-id="448d3-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="448d3-110">获取员工</span><span class="sxs-lookup"><span data-stu-id="448d3-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="448d3-111">employees</span><span class="sxs-lookup"><span data-stu-id="448d3-111">employees</span></span>  |<span data-ttu-id="448d3-112">获取 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="448d3-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="448d3-113">发布员工</span><span class="sxs-lookup"><span data-stu-id="448d3-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="448d3-114">employees</span><span class="sxs-lookup"><span data-stu-id="448d3-114">employees</span></span>  |<span data-ttu-id="448d3-115">创建 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="448d3-115">Create an employee object.</span></span>|
|[<span data-ttu-id="448d3-116">修补员工</span><span class="sxs-lookup"><span data-stu-id="448d3-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="448d3-117">employees</span><span class="sxs-lookup"><span data-stu-id="448d3-117">employees</span></span>  |<span data-ttu-id="448d3-118">更新 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="448d3-118">Update an employee object.</span></span>|
|[<span data-ttu-id="448d3-119">删除员工</span><span class="sxs-lookup"><span data-stu-id="448d3-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="448d3-120">无</span><span class="sxs-lookup"><span data-stu-id="448d3-120">none</span></span>       |<span data-ttu-id="448d3-121">删除 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="448d3-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="448d3-122">属性</span><span class="sxs-lookup"><span data-stu-id="448d3-122">Properties</span></span>
| <span data-ttu-id="448d3-123">属性</span><span class="sxs-lookup"><span data-stu-id="448d3-123">Property</span></span>           | <span data-ttu-id="448d3-124">类型</span><span class="sxs-lookup"><span data-stu-id="448d3-124">Type</span></span>   |<span data-ttu-id="448d3-125">说明</span><span class="sxs-lookup"><span data-stu-id="448d3-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="448d3-126">id</span><span class="sxs-lookup"><span data-stu-id="448d3-126">id</span></span>                  |<span data-ttu-id="448d3-127">GUID</span><span class="sxs-lookup"><span data-stu-id="448d3-127">GUID</span></span>    |<span data-ttu-id="448d3-128">员工 ID。</span><span class="sxs-lookup"><span data-stu-id="448d3-128">The employee ID.</span></span> <span data-ttu-id="448d3-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="448d3-129">Non-editable.</span></span>                         |
|<span data-ttu-id="448d3-130">number</span><span class="sxs-lookup"><span data-stu-id="448d3-130">number</span></span>              |<span data-ttu-id="448d3-131">string</span><span class="sxs-lookup"><span data-stu-id="448d3-131">string</span></span>  |<span data-ttu-id="448d3-132">员工编号。</span><span class="sxs-lookup"><span data-stu-id="448d3-132">The employee number.</span></span> <span data-ttu-id="448d3-133">只读。</span><span class="sxs-lookup"><span data-stu-id="448d3-133">Read-Only.</span></span>                        |
|<span data-ttu-id="448d3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="448d3-134">displayName</span></span>         |<span data-ttu-id="448d3-135">string</span><span class="sxs-lookup"><span data-stu-id="448d3-135">string</span></span>  |<span data-ttu-id="448d3-136">雇员 givenName + surname。</span><span class="sxs-lookup"><span data-stu-id="448d3-136">The employee givenName + surname.</span></span> <span data-ttu-id="448d3-137">只读。</span><span class="sxs-lookup"><span data-stu-id="448d3-137">Read-Only.</span></span>           |
|<span data-ttu-id="448d3-138">givenName</span><span class="sxs-lookup"><span data-stu-id="448d3-138">givenName</span></span>           |<span data-ttu-id="448d3-139">string</span><span class="sxs-lookup"><span data-stu-id="448d3-139">string</span></span>  |<span data-ttu-id="448d3-140">雇员的给定名称。</span><span class="sxs-lookup"><span data-stu-id="448d3-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="448d3-141">middleName</span><span class="sxs-lookup"><span data-stu-id="448d3-141">middleName</span></span>          |<span data-ttu-id="448d3-142">string</span><span class="sxs-lookup"><span data-stu-id="448d3-142">string</span></span>  |<span data-ttu-id="448d3-143">员工的中间名。</span><span class="sxs-lookup"><span data-stu-id="448d3-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="448d3-144">surname</span><span class="sxs-lookup"><span data-stu-id="448d3-144">surname</span></span>             |<span data-ttu-id="448d3-145">string</span><span class="sxs-lookup"><span data-stu-id="448d3-145">string</span></span>  |<span data-ttu-id="448d3-146">员工的姓氏</span><span class="sxs-lookup"><span data-stu-id="448d3-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="448d3-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="448d3-147">jobTitle</span></span>            |<span data-ttu-id="448d3-148">string</span><span class="sxs-lookup"><span data-stu-id="448d3-148">string</span></span>  |<span data-ttu-id="448d3-149">员工职务</span><span class="sxs-lookup"><span data-stu-id="448d3-149">The job title of the employee</span></span>                          |
|<span data-ttu-id="448d3-150">address</span><span class="sxs-lookup"><span data-stu-id="448d3-150">address</span></span>             |[<span data-ttu-id="448d3-151">导航。PostalAddress</span><span class="sxs-lookup"><span data-stu-id="448d3-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="448d3-152">指定员工的地址。</span><span class="sxs-lookup"><span data-stu-id="448d3-152">Specifies the employee's address.</span></span> <span data-ttu-id="448d3-153">此地址将显示在员工的所有资源文档上。</span><span class="sxs-lookup"><span data-stu-id="448d3-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="448d3-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="448d3-154">phoneNumber</span></span>         |<span data-ttu-id="448d3-155">string</span><span class="sxs-lookup"><span data-stu-id="448d3-155">string</span></span>  |<span data-ttu-id="448d3-156">指定员工的电话号码。</span><span class="sxs-lookup"><span data-stu-id="448d3-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="448d3-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="448d3-157">mobilePhone</span></span>         |<span data-ttu-id="448d3-158">string</span><span class="sxs-lookup"><span data-stu-id="448d3-158">string</span></span>  |<span data-ttu-id="448d3-159">指定员工的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="448d3-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="448d3-160">email</span><span class="sxs-lookup"><span data-stu-id="448d3-160">email</span></span>               |<span data-ttu-id="448d3-161">string</span><span class="sxs-lookup"><span data-stu-id="448d3-161">string</span></span>  |<span data-ttu-id="448d3-162">指定员工的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="448d3-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="448d3-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="448d3-163">personalEmail</span></span>       |<span data-ttu-id="448d3-164">string</span><span class="sxs-lookup"><span data-stu-id="448d3-164">string</span></span>  |<span data-ttu-id="448d3-165">指定员工的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="448d3-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="448d3-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="448d3-166">employmentDate</span></span>      |<span data-ttu-id="448d3-167">date</span><span class="sxs-lookup"><span data-stu-id="448d3-167">date</span></span>    |<span data-ttu-id="448d3-168">指定员工开始为公司工作的日期。</span><span class="sxs-lookup"><span data-stu-id="448d3-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="448d3-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="448d3-169">terminationDate</span></span>     |<span data-ttu-id="448d3-170">date</span><span class="sxs-lookup"><span data-stu-id="448d3-170">date</span></span>    |<span data-ttu-id="448d3-171">例如，指定员工因停用或离职而终止的日期。</span><span class="sxs-lookup"><span data-stu-id="448d3-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="448d3-172">状态</span><span class="sxs-lookup"><span data-stu-id="448d3-172">status</span></span>              |<span data-ttu-id="448d3-173">string</span><span class="sxs-lookup"><span data-stu-id="448d3-173">string</span></span>  |<span data-ttu-id="448d3-174">指定员工的状态。</span><span class="sxs-lookup"><span data-stu-id="448d3-174">Specifies the employee's status.</span></span> <span data-ttu-id="448d3-175">可能的值是 Active、Inactive 或 Terminated</span><span class="sxs-lookup"><span data-stu-id="448d3-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="448d3-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="448d3-176">birthDate</span></span>           |<span data-ttu-id="448d3-177">date</span><span class="sxs-lookup"><span data-stu-id="448d3-177">date</span></span>    |<span data-ttu-id="448d3-178">指定员工出生日期。</span><span class="sxs-lookup"><span data-stu-id="448d3-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="448d3-179">picture</span><span class="sxs-lookup"><span data-stu-id="448d3-179">picture</span></span>             |<span data-ttu-id="448d3-180">stream</span><span class="sxs-lookup"><span data-stu-id="448d3-180">stream</span></span>  |<span data-ttu-id="448d3-181">员工图片。</span><span class="sxs-lookup"><span data-stu-id="448d3-181">The employee picture.</span></span> <span data-ttu-id="448d3-182">只读。</span><span class="sxs-lookup"><span data-stu-id="448d3-182">Read-Only.</span></span>                       |
|<span data-ttu-id="448d3-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="448d3-183">lastModifiedDateTime</span></span>|<span data-ttu-id="448d3-184">datetime</span><span class="sxs-lookup"><span data-stu-id="448d3-184">datetime</span></span>|<span data-ttu-id="448d3-185">上次修改员工的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="448d3-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="448d3-186">只读。</span><span class="sxs-lookup"><span data-stu-id="448d3-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="448d3-187">关系</span><span class="sxs-lookup"><span data-stu-id="448d3-187">Relationships</span></span>
<span data-ttu-id="448d3-188">无</span><span class="sxs-lookup"><span data-stu-id="448d3-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="448d3-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="448d3-189">JSON representation</span></span>

<span data-ttu-id="448d3-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="448d3-190">Here is a JSON representation of the resource.</span></span>


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



