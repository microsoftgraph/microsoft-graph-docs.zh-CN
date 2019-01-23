---
title: termsAndConditionsAcceptanceStatus 资源类型
description: termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e6156c1f5cf952f485e6f0a210a7aef4bd7b3ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412553"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="1363e-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="1363e-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="1363e-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1363e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1363e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1363e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1363e-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1363e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1363e-108">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="1363e-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="1363e-109">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="1363e-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="1363e-110">方法</span><span class="sxs-lookup"><span data-stu-id="1363e-110">Methods</span></span>
|<span data-ttu-id="1363e-111">方法</span><span class="sxs-lookup"><span data-stu-id="1363e-111">Method</span></span>|<span data-ttu-id="1363e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1363e-112">Return Type</span></span>|<span data-ttu-id="1363e-113">说明</span><span class="sxs-lookup"><span data-stu-id="1363e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1363e-114">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="1363e-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="1363e-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1363e-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="1363e-116">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1363e-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="1363e-117">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="1363e-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="1363e-119">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1363e-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="1363e-120">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="1363e-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="1363e-122">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1363e-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="1363e-123">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="1363e-124">无</span><span class="sxs-lookup"><span data-stu-id="1363e-124">None</span></span>|<span data-ttu-id="1363e-125">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="1363e-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="1363e-126">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="1363e-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1363e-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="1363e-128">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1363e-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1363e-129">属性</span><span class="sxs-lookup"><span data-stu-id="1363e-129">Properties</span></span>
|<span data-ttu-id="1363e-130">属性</span><span class="sxs-lookup"><span data-stu-id="1363e-130">Property</span></span>|<span data-ttu-id="1363e-131">类型</span><span class="sxs-lookup"><span data-stu-id="1363e-131">Type</span></span>|<span data-ttu-id="1363e-132">说明</span><span class="sxs-lookup"><span data-stu-id="1363e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1363e-133">id</span><span class="sxs-lookup"><span data-stu-id="1363e-133">id</span></span>|<span data-ttu-id="1363e-134">String</span><span class="sxs-lookup"><span data-stu-id="1363e-134">String</span></span>|<span data-ttu-id="1363e-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1363e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1363e-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1363e-136">userDisplayName</span></span>|<span data-ttu-id="1363e-137">String</span><span class="sxs-lookup"><span data-stu-id="1363e-137">String</span></span>|<span data-ttu-id="1363e-138">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1363e-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="1363e-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="1363e-139">acceptedVersion</span></span>|<span data-ttu-id="1363e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1363e-140">Int32</span></span>|<span data-ttu-id="1363e-141">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="1363e-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="1363e-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="1363e-142">acceptedDateTime</span></span>|<span data-ttu-id="1363e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1363e-143">DateTimeOffset</span></span>|<span data-ttu-id="1363e-144">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1363e-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1363e-145">关系</span><span class="sxs-lookup"><span data-stu-id="1363e-145">Relationships</span></span>
|<span data-ttu-id="1363e-146">关系</span><span class="sxs-lookup"><span data-stu-id="1363e-146">Relationship</span></span>|<span data-ttu-id="1363e-147">类型</span><span class="sxs-lookup"><span data-stu-id="1363e-147">Type</span></span>|<span data-ttu-id="1363e-148">说明</span><span class="sxs-lookup"><span data-stu-id="1363e-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1363e-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1363e-149">termsAndConditions</span></span>|[<span data-ttu-id="1363e-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1363e-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="1363e-151">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="1363e-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1363e-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1363e-152">JSON Representation</span></span>
<span data-ttu-id="1363e-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1363e-153">Here is a JSON representation of the resource.</span></span>
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




