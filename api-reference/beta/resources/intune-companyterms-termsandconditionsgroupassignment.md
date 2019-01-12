---
title: termsAndConditionsGroupAssignment 资源类型
description: C） 到给定的组策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3efd219e175743afdca35d1b4348de0c6f571540
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954111"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="102ee-104">termsAndConditionsGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="102ee-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="102ee-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="102ee-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="102ee-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="102ee-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="102ee-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="102ee-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="102ee-108">TermsAndConditionsGroupAssignment 实体表示给定条款和条件 (T & C) 策略分配到给定的组。</span><span class="sxs-lookup"><span data-stu-id="102ee-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="102ee-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="102ee-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="102ee-110">方法</span><span class="sxs-lookup"><span data-stu-id="102ee-110">Methods</span></span>
|<span data-ttu-id="102ee-111">方法</span><span class="sxs-lookup"><span data-stu-id="102ee-111">Method</span></span>|<span data-ttu-id="102ee-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="102ee-112">Return Type</span></span>|<span data-ttu-id="102ee-113">说明</span><span class="sxs-lookup"><span data-stu-id="102ee-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="102ee-114">列表 termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="102ee-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="102ee-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="102ee-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="102ee-116">列出属性和[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="102ee-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="102ee-117">获取 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="102ee-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="102ee-119">读取属性和[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="102ee-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="102ee-120">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="102ee-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="102ee-122">创建新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="102ee-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="102ee-123">删除 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="102ee-124">无</span><span class="sxs-lookup"><span data-stu-id="102ee-124">None</span></span>|<span data-ttu-id="102ee-125">删除[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="102ee-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="102ee-126">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="102ee-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="102ee-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="102ee-128">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="102ee-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="102ee-129">属性</span><span class="sxs-lookup"><span data-stu-id="102ee-129">Properties</span></span>
|<span data-ttu-id="102ee-130">属性</span><span class="sxs-lookup"><span data-stu-id="102ee-130">Property</span></span>|<span data-ttu-id="102ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="102ee-131">Type</span></span>|<span data-ttu-id="102ee-132">说明</span><span class="sxs-lookup"><span data-stu-id="102ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102ee-133">id</span><span class="sxs-lookup"><span data-stu-id="102ee-133">id</span></span>|<span data-ttu-id="102ee-134">String</span><span class="sxs-lookup"><span data-stu-id="102ee-134">String</span></span>|<span data-ttu-id="102ee-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="102ee-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="102ee-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="102ee-136">targetGroupId</span></span>|<span data-ttu-id="102ee-137">字符串</span><span class="sxs-lookup"><span data-stu-id="102ee-137">String</span></span>|<span data-ttu-id="102ee-138">T & C 策略分配给组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="102ee-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="102ee-139">Relationships</span><span class="sxs-lookup"><span data-stu-id="102ee-139">Relationships</span></span>
|<span data-ttu-id="102ee-140">关系</span><span class="sxs-lookup"><span data-stu-id="102ee-140">Relationship</span></span>|<span data-ttu-id="102ee-141">类型</span><span class="sxs-lookup"><span data-stu-id="102ee-141">Type</span></span>|<span data-ttu-id="102ee-142">说明</span><span class="sxs-lookup"><span data-stu-id="102ee-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102ee-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="102ee-143">termsAndConditions</span></span>|[<span data-ttu-id="102ee-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="102ee-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="102ee-145">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="102ee-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="102ee-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="102ee-146">JSON Representation</span></span>
<span data-ttu-id="102ee-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="102ee-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





