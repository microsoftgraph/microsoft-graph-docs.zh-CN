---
title: termsAndConditionsAcceptanceStatus 资源类型
description: termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2809ab80228fd65c491c6dd232e90e253de839b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024379"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="d8cff-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8cff-104">termsAndConditionsAcceptanceStatus resource type</span></span>

<span data-ttu-id="d8cff-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8cff-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8cff-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8cff-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8cff-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8cff-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8cff-108">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="d8cff-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="d8cff-109">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d8cff-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="d8cff-110">方法</span><span class="sxs-lookup"><span data-stu-id="d8cff-110">Methods</span></span>
|<span data-ttu-id="d8cff-111">方法</span><span class="sxs-lookup"><span data-stu-id="d8cff-111">Method</span></span>|<span data-ttu-id="d8cff-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8cff-112">Return Type</span></span>|<span data-ttu-id="d8cff-113">说明</span><span class="sxs-lookup"><span data-stu-id="d8cff-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8cff-114">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="d8cff-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="d8cff-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8cff-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="d8cff-116">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8cff-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="d8cff-117">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="d8cff-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="d8cff-119">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8cff-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="d8cff-120">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="d8cff-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="d8cff-122">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8cff-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="d8cff-123">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="d8cff-124">无</span><span class="sxs-lookup"><span data-stu-id="d8cff-124">None</span></span>|<span data-ttu-id="d8cff-125">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="d8cff-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="d8cff-126">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="d8cff-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d8cff-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="d8cff-128">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8cff-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8cff-129">属性</span><span class="sxs-lookup"><span data-stu-id="d8cff-129">Properties</span></span>
|<span data-ttu-id="d8cff-130">属性</span><span class="sxs-lookup"><span data-stu-id="d8cff-130">Property</span></span>|<span data-ttu-id="d8cff-131">类型</span><span class="sxs-lookup"><span data-stu-id="d8cff-131">Type</span></span>|<span data-ttu-id="d8cff-132">说明</span><span class="sxs-lookup"><span data-stu-id="d8cff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8cff-133">id</span><span class="sxs-lookup"><span data-stu-id="d8cff-133">id</span></span>|<span data-ttu-id="d8cff-134">String</span><span class="sxs-lookup"><span data-stu-id="d8cff-134">String</span></span>|<span data-ttu-id="d8cff-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d8cff-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d8cff-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8cff-136">userDisplayName</span></span>|<span data-ttu-id="d8cff-137">String</span><span class="sxs-lookup"><span data-stu-id="d8cff-137">String</span></span>|<span data-ttu-id="d8cff-138">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d8cff-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="d8cff-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="d8cff-139">acceptedVersion</span></span>|<span data-ttu-id="d8cff-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d8cff-140">Int32</span></span>|<span data-ttu-id="d8cff-141">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="d8cff-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="d8cff-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8cff-142">acceptedDateTime</span></span>|<span data-ttu-id="d8cff-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8cff-143">DateTimeOffset</span></span>|<span data-ttu-id="d8cff-144">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8cff-144">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="d8cff-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8cff-145">userPrincipalName</span></span>|<span data-ttu-id="d8cff-146">String</span><span class="sxs-lookup"><span data-stu-id="d8cff-146">String</span></span>|<span data-ttu-id="d8cff-147">接受术语的用户的 userPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d8cff-147">The userPrincipalName of the User that accepted the term.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8cff-148">关系</span><span class="sxs-lookup"><span data-stu-id="d8cff-148">Relationships</span></span>
|<span data-ttu-id="d8cff-149">关系</span><span class="sxs-lookup"><span data-stu-id="d8cff-149">Relationship</span></span>|<span data-ttu-id="d8cff-150">类型</span><span class="sxs-lookup"><span data-stu-id="d8cff-150">Type</span></span>|<span data-ttu-id="d8cff-151">说明</span><span class="sxs-lookup"><span data-stu-id="d8cff-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8cff-152">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d8cff-152">termsAndConditions</span></span>|[<span data-ttu-id="d8cff-153">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d8cff-153">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="d8cff-154">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="d8cff-154">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8cff-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8cff-155">JSON Representation</span></span>
<span data-ttu-id="d8cff-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8cff-156">Here is a JSON representation of the resource.</span></span>
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
  "acceptedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```






