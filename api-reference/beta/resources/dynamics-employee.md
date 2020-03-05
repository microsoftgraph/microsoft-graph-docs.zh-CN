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
# <a name="employees-resource-type"></a><span data-ttu-id="44afe-103">员工资源类型</span><span class="sxs-lookup"><span data-stu-id="44afe-103">employees resource type</span></span>

<span data-ttu-id="44afe-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="44afe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44afe-105">表示 Dynamics 365 Business Central 中的员工。</span><span class="sxs-lookup"><span data-stu-id="44afe-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="44afe-106">方法</span><span class="sxs-lookup"><span data-stu-id="44afe-106">Methods</span></span>

| <span data-ttu-id="44afe-107">方法</span><span class="sxs-lookup"><span data-stu-id="44afe-107">Method</span></span>                                              | <span data-ttu-id="44afe-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="44afe-108">Return Type</span></span>|<span data-ttu-id="44afe-109">说明</span><span class="sxs-lookup"><span data-stu-id="44afe-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="44afe-110">获取员工</span><span class="sxs-lookup"><span data-stu-id="44afe-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="44afe-111">员工</span><span class="sxs-lookup"><span data-stu-id="44afe-111">employees</span></span>  |<span data-ttu-id="44afe-112">获取一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="44afe-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="44afe-113">过帐员工</span><span class="sxs-lookup"><span data-stu-id="44afe-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="44afe-114">员工</span><span class="sxs-lookup"><span data-stu-id="44afe-114">employees</span></span>  |<span data-ttu-id="44afe-115">创建一个 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="44afe-115">Create an employee object.</span></span>|
|[<span data-ttu-id="44afe-116">修补员工</span><span class="sxs-lookup"><span data-stu-id="44afe-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="44afe-117">员工</span><span class="sxs-lookup"><span data-stu-id="44afe-117">employees</span></span>  |<span data-ttu-id="44afe-118">更新 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="44afe-118">Update an employee object.</span></span>|
|[<span data-ttu-id="44afe-119">删除员工</span><span class="sxs-lookup"><span data-stu-id="44afe-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="44afe-120">无</span><span class="sxs-lookup"><span data-stu-id="44afe-120">none</span></span>       |<span data-ttu-id="44afe-121">删除 employee 对象。</span><span class="sxs-lookup"><span data-stu-id="44afe-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44afe-122">属性</span><span class="sxs-lookup"><span data-stu-id="44afe-122">Properties</span></span>
| <span data-ttu-id="44afe-123">属性</span><span class="sxs-lookup"><span data-stu-id="44afe-123">Property</span></span>           | <span data-ttu-id="44afe-124">类型</span><span class="sxs-lookup"><span data-stu-id="44afe-124">Type</span></span>   |<span data-ttu-id="44afe-125">说明</span><span class="sxs-lookup"><span data-stu-id="44afe-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="44afe-126">id</span><span class="sxs-lookup"><span data-stu-id="44afe-126">id</span></span>                  |<span data-ttu-id="44afe-127">GUID</span><span class="sxs-lookup"><span data-stu-id="44afe-127">GUID</span></span>    |<span data-ttu-id="44afe-128">员工 ID。</span><span class="sxs-lookup"><span data-stu-id="44afe-128">The employee ID.</span></span> <span data-ttu-id="44afe-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="44afe-129">Non-editable.</span></span>                         |
|<span data-ttu-id="44afe-130">number</span><span class="sxs-lookup"><span data-stu-id="44afe-130">number</span></span>              |<span data-ttu-id="44afe-131">string</span><span class="sxs-lookup"><span data-stu-id="44afe-131">string</span></span>  |<span data-ttu-id="44afe-132">员工编号。</span><span class="sxs-lookup"><span data-stu-id="44afe-132">The employee number.</span></span> <span data-ttu-id="44afe-133">只读。</span><span class="sxs-lookup"><span data-stu-id="44afe-133">Read-Only.</span></span>                        |
|<span data-ttu-id="44afe-134">displayName</span><span class="sxs-lookup"><span data-stu-id="44afe-134">displayName</span></span>         |<span data-ttu-id="44afe-135">string</span><span class="sxs-lookup"><span data-stu-id="44afe-135">string</span></span>  |<span data-ttu-id="44afe-136">员工 givenName + 姓。</span><span class="sxs-lookup"><span data-stu-id="44afe-136">The employee givenName + surname.</span></span> <span data-ttu-id="44afe-137">只读。</span><span class="sxs-lookup"><span data-stu-id="44afe-137">Read-Only.</span></span>           |
|<span data-ttu-id="44afe-138">givenName</span><span class="sxs-lookup"><span data-stu-id="44afe-138">givenName</span></span>           |<span data-ttu-id="44afe-139">string</span><span class="sxs-lookup"><span data-stu-id="44afe-139">string</span></span>  |<span data-ttu-id="44afe-140">员工的名字。</span><span class="sxs-lookup"><span data-stu-id="44afe-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="44afe-141">middleName</span><span class="sxs-lookup"><span data-stu-id="44afe-141">middleName</span></span>          |<span data-ttu-id="44afe-142">string</span><span class="sxs-lookup"><span data-stu-id="44afe-142">string</span></span>  |<span data-ttu-id="44afe-143">员工的中间名。</span><span class="sxs-lookup"><span data-stu-id="44afe-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="44afe-144">surname</span><span class="sxs-lookup"><span data-stu-id="44afe-144">surname</span></span>             |<span data-ttu-id="44afe-145">string</span><span class="sxs-lookup"><span data-stu-id="44afe-145">string</span></span>  |<span data-ttu-id="44afe-146">员工的姓氏</span><span class="sxs-lookup"><span data-stu-id="44afe-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="44afe-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="44afe-147">jobTitle</span></span>            |<span data-ttu-id="44afe-148">string</span><span class="sxs-lookup"><span data-stu-id="44afe-148">string</span></span>  |<span data-ttu-id="44afe-149">员工的完整名称</span><span class="sxs-lookup"><span data-stu-id="44afe-149">The full name of the employee</span></span>                          |
|<span data-ttu-id="44afe-150">address</span><span class="sxs-lookup"><span data-stu-id="44afe-150">address</span></span>             |[<span data-ttu-id="44afe-151">翻.省略</span><span class="sxs-lookup"><span data-stu-id="44afe-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="44afe-152">指定员工的地址。</span><span class="sxs-lookup"><span data-stu-id="44afe-152">Specifies the employee's address.</span></span> <span data-ttu-id="44afe-153">此地址将显示在员工的所有资源文档中。</span><span class="sxs-lookup"><span data-stu-id="44afe-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="44afe-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="44afe-154">phoneNumber</span></span>         |<span data-ttu-id="44afe-155">string</span><span class="sxs-lookup"><span data-stu-id="44afe-155">string</span></span>  |<span data-ttu-id="44afe-156">指定员工的电话号码。</span><span class="sxs-lookup"><span data-stu-id="44afe-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="44afe-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="44afe-157">mobilePhone</span></span>         |<span data-ttu-id="44afe-158">string</span><span class="sxs-lookup"><span data-stu-id="44afe-158">string</span></span>  |<span data-ttu-id="44afe-159">指定员工的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="44afe-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="44afe-160">email</span><span class="sxs-lookup"><span data-stu-id="44afe-160">email</span></span>               |<span data-ttu-id="44afe-161">string</span><span class="sxs-lookup"><span data-stu-id="44afe-161">string</span></span>  |<span data-ttu-id="44afe-162">指定员工的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="44afe-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="44afe-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="44afe-163">personalEmail</span></span>       |<span data-ttu-id="44afe-164">string</span><span class="sxs-lookup"><span data-stu-id="44afe-164">string</span></span>  |<span data-ttu-id="44afe-165">指定员工的个人电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="44afe-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="44afe-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="44afe-166">employmentDate</span></span>      |<span data-ttu-id="44afe-167">date</span><span class="sxs-lookup"><span data-stu-id="44afe-167">date</span></span>    |<span data-ttu-id="44afe-168">指定员工开始为公司工作的日期。</span><span class="sxs-lookup"><span data-stu-id="44afe-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="44afe-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="44afe-169">terminationDate</span></span>     |<span data-ttu-id="44afe-170">date</span><span class="sxs-lookup"><span data-stu-id="44afe-170">date</span></span>    |<span data-ttu-id="44afe-171">指定由于退休或开除而终止员工的日期。</span><span class="sxs-lookup"><span data-stu-id="44afe-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="44afe-172">状态</span><span class="sxs-lookup"><span data-stu-id="44afe-172">status</span></span>              |<span data-ttu-id="44afe-173">string</span><span class="sxs-lookup"><span data-stu-id="44afe-173">string</span></span>  |<span data-ttu-id="44afe-174">指定员工的状态。</span><span class="sxs-lookup"><span data-stu-id="44afe-174">Specifies the employee's status.</span></span> <span data-ttu-id="44afe-175">可能的值包括活动、非活动或已终止</span><span class="sxs-lookup"><span data-stu-id="44afe-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="44afe-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="44afe-176">birthDate</span></span>           |<span data-ttu-id="44afe-177">date</span><span class="sxs-lookup"><span data-stu-id="44afe-177">date</span></span>    |<span data-ttu-id="44afe-178">指定员工的出生日期。</span><span class="sxs-lookup"><span data-stu-id="44afe-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="44afe-179">头像</span><span class="sxs-lookup"><span data-stu-id="44afe-179">picture</span></span>             |<span data-ttu-id="44afe-180">stream</span><span class="sxs-lookup"><span data-stu-id="44afe-180">stream</span></span>  |<span data-ttu-id="44afe-181">员工头像。</span><span class="sxs-lookup"><span data-stu-id="44afe-181">The employee picture.</span></span> <span data-ttu-id="44afe-182">只读。</span><span class="sxs-lookup"><span data-stu-id="44afe-182">Read-Only.</span></span>                       |
|<span data-ttu-id="44afe-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44afe-183">lastModifiedDateTime</span></span>|<span data-ttu-id="44afe-184">datetime</span><span class="sxs-lookup"><span data-stu-id="44afe-184">datetime</span></span>|<span data-ttu-id="44afe-185">上次修改员工的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="44afe-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="44afe-186">只读。</span><span class="sxs-lookup"><span data-stu-id="44afe-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="44afe-187">关系</span><span class="sxs-lookup"><span data-stu-id="44afe-187">Relationships</span></span>
<span data-ttu-id="44afe-188">无</span><span class="sxs-lookup"><span data-stu-id="44afe-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44afe-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44afe-189">JSON representation</span></span>

<span data-ttu-id="44afe-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44afe-190">Here is a JSON representation of the resource.</span></span>


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

