---
title: termsAndConditionsAcceptanceStatus 资源类型
description: termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3df5a81870729fba79519be4010c852aa6810f50
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251046"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="e2302-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2302-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="e2302-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2302-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2302-106">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="e2302-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="e2302-107">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e2302-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="e2302-108">方法</span><span class="sxs-lookup"><span data-stu-id="e2302-108">Methods</span></span>
|<span data-ttu-id="e2302-109">方法</span><span class="sxs-lookup"><span data-stu-id="e2302-109">Method</span></span>|<span data-ttu-id="e2302-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2302-110">Return Type</span></span>|<span data-ttu-id="e2302-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2302-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2302-112">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="e2302-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="e2302-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2302-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="e2302-114">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2302-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="e2302-115">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="e2302-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="e2302-117">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2302-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="e2302-118">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="e2302-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="e2302-120">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2302-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="e2302-121">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="e2302-122">无</span><span class="sxs-lookup"><span data-stu-id="e2302-122">None</span></span>|<span data-ttu-id="e2302-123">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="e2302-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="e2302-124">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="e2302-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e2302-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="e2302-126">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e2302-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2302-127">属性</span><span class="sxs-lookup"><span data-stu-id="e2302-127">Properties</span></span>
|<span data-ttu-id="e2302-128">属性</span><span class="sxs-lookup"><span data-stu-id="e2302-128">Property</span></span>|<span data-ttu-id="e2302-129">类型</span><span class="sxs-lookup"><span data-stu-id="e2302-129">Type</span></span>|<span data-ttu-id="e2302-130">说明</span><span class="sxs-lookup"><span data-stu-id="e2302-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2302-131">id</span><span class="sxs-lookup"><span data-stu-id="e2302-131">id</span></span>|<span data-ttu-id="e2302-132">String</span><span class="sxs-lookup"><span data-stu-id="e2302-132">String</span></span>|<span data-ttu-id="e2302-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e2302-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e2302-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e2302-134">userDisplayName</span></span>|<span data-ttu-id="e2302-135">String</span><span class="sxs-lookup"><span data-stu-id="e2302-135">String</span></span>|<span data-ttu-id="e2302-136">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e2302-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="e2302-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="e2302-137">acceptedVersion</span></span>|<span data-ttu-id="e2302-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e2302-138">Int32</span></span>|<span data-ttu-id="e2302-139">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="e2302-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="e2302-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2302-140">acceptedDateTime</span></span>|<span data-ttu-id="e2302-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2302-141">DateTimeOffset</span></span>|<span data-ttu-id="e2302-142">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e2302-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2302-143">关系</span><span class="sxs-lookup"><span data-stu-id="e2302-143">Relationships</span></span>
|<span data-ttu-id="e2302-144">关系</span><span class="sxs-lookup"><span data-stu-id="e2302-144">Relationship</span></span>|<span data-ttu-id="e2302-145">类型</span><span class="sxs-lookup"><span data-stu-id="e2302-145">Type</span></span>|<span data-ttu-id="e2302-146">说明</span><span class="sxs-lookup"><span data-stu-id="e2302-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2302-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e2302-147">termsAndConditions</span></span>|[<span data-ttu-id="e2302-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e2302-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="e2302-149">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="e2302-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2302-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2302-150">JSON Representation</span></span>
<span data-ttu-id="e2302-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2302-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



