---
title: termsAndConditionsAcceptanceStatus 资源类型
description: termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6381f40f5b9abea76da84930894f83d3da8fb3c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949148"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="68f39-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="68f39-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="68f39-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68f39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68f39-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68f39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68f39-107">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="68f39-107">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="68f39-108">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="68f39-108">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="68f39-109">方法</span><span class="sxs-lookup"><span data-stu-id="68f39-109">Methods</span></span>
|<span data-ttu-id="68f39-110">方法</span><span class="sxs-lookup"><span data-stu-id="68f39-110">Method</span></span>|<span data-ttu-id="68f39-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="68f39-111">Return Type</span></span>|<span data-ttu-id="68f39-112">说明</span><span class="sxs-lookup"><span data-stu-id="68f39-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68f39-113">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="68f39-113">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="68f39-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68f39-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="68f39-115">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="68f39-115">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="68f39-116">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-116">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="68f39-117">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-117">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="68f39-118">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="68f39-118">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="68f39-119">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-119">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="68f39-120">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-120">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="68f39-121">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68f39-121">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="68f39-122">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-122">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="68f39-123">无</span><span class="sxs-lookup"><span data-stu-id="68f39-123">None</span></span>|<span data-ttu-id="68f39-124">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="68f39-124">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="68f39-125">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-125">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="68f39-126">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="68f39-126">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="68f39-127">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="68f39-127">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68f39-128">属性</span><span class="sxs-lookup"><span data-stu-id="68f39-128">Properties</span></span>
|<span data-ttu-id="68f39-129">属性</span><span class="sxs-lookup"><span data-stu-id="68f39-129">Property</span></span>|<span data-ttu-id="68f39-130">类型</span><span class="sxs-lookup"><span data-stu-id="68f39-130">Type</span></span>|<span data-ttu-id="68f39-131">说明</span><span class="sxs-lookup"><span data-stu-id="68f39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f39-132">id</span><span class="sxs-lookup"><span data-stu-id="68f39-132">id</span></span>|<span data-ttu-id="68f39-133">字符串</span><span class="sxs-lookup"><span data-stu-id="68f39-133">String</span></span>|<span data-ttu-id="68f39-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="68f39-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="68f39-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="68f39-135">userDisplayName</span></span>|<span data-ttu-id="68f39-136">String</span><span class="sxs-lookup"><span data-stu-id="68f39-136">String</span></span>|<span data-ttu-id="68f39-137">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="68f39-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="68f39-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="68f39-138">acceptedVersion</span></span>|<span data-ttu-id="68f39-139">Int32</span><span class="sxs-lookup"><span data-stu-id="68f39-139">Int32</span></span>|<span data-ttu-id="68f39-140">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="68f39-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="68f39-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="68f39-141">acceptedDateTime</span></span>|<span data-ttu-id="68f39-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68f39-142">DateTimeOffset</span></span>|<span data-ttu-id="68f39-143">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="68f39-143">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68f39-144">关系</span><span class="sxs-lookup"><span data-stu-id="68f39-144">Relationships</span></span>
|<span data-ttu-id="68f39-145">关系</span><span class="sxs-lookup"><span data-stu-id="68f39-145">Relationship</span></span>|<span data-ttu-id="68f39-146">类型</span><span class="sxs-lookup"><span data-stu-id="68f39-146">Type</span></span>|<span data-ttu-id="68f39-147">说明</span><span class="sxs-lookup"><span data-stu-id="68f39-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f39-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="68f39-148">termsAndConditions</span></span>|[<span data-ttu-id="68f39-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="68f39-149">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="68f39-150">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="68f39-150">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68f39-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68f39-151">JSON Representation</span></span>
<span data-ttu-id="68f39-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68f39-152">Here is a JSON representation of the resource.</span></span>
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




