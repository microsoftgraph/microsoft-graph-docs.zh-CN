---
title: termsAndConditionsAcceptanceStatus 资源类型
description: termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d3e007c260e308b3c86ae6bba95b11d362d0f40
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758930"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="f93ac-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f93ac-104">termsAndConditionsAcceptanceStatus resource type</span></span>

<span data-ttu-id="f93ac-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f93ac-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f93ac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f93ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f93ac-107">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="f93ac-107">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="f93ac-108">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f93ac-108">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="f93ac-109">方法</span><span class="sxs-lookup"><span data-stu-id="f93ac-109">Methods</span></span>
|<span data-ttu-id="f93ac-110">方法</span><span class="sxs-lookup"><span data-stu-id="f93ac-110">Method</span></span>|<span data-ttu-id="f93ac-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f93ac-111">Return Type</span></span>|<span data-ttu-id="f93ac-112">说明</span><span class="sxs-lookup"><span data-stu-id="f93ac-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f93ac-113">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="f93ac-113">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="f93ac-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f93ac-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="f93ac-115">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f93ac-115">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="f93ac-116">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-116">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="f93ac-117">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-117">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="f93ac-118">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f93ac-118">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="f93ac-119">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-119">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="f93ac-120">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-120">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="f93ac-121">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f93ac-121">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="f93ac-122">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-122">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="f93ac-123">无</span><span class="sxs-lookup"><span data-stu-id="f93ac-123">None</span></span>|<span data-ttu-id="f93ac-124">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="f93ac-124">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="f93ac-125">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-125">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="f93ac-126">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f93ac-126">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="f93ac-127">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f93ac-127">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f93ac-128">属性</span><span class="sxs-lookup"><span data-stu-id="f93ac-128">Properties</span></span>
|<span data-ttu-id="f93ac-129">属性</span><span class="sxs-lookup"><span data-stu-id="f93ac-129">Property</span></span>|<span data-ttu-id="f93ac-130">类型</span><span class="sxs-lookup"><span data-stu-id="f93ac-130">Type</span></span>|<span data-ttu-id="f93ac-131">说明</span><span class="sxs-lookup"><span data-stu-id="f93ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93ac-132">id</span><span class="sxs-lookup"><span data-stu-id="f93ac-132">id</span></span>|<span data-ttu-id="f93ac-133">String</span><span class="sxs-lookup"><span data-stu-id="f93ac-133">String</span></span>|<span data-ttu-id="f93ac-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f93ac-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f93ac-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f93ac-135">userDisplayName</span></span>|<span data-ttu-id="f93ac-136">String</span><span class="sxs-lookup"><span data-stu-id="f93ac-136">String</span></span>|<span data-ttu-id="f93ac-137">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f93ac-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="f93ac-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="f93ac-138">acceptedVersion</span></span>|<span data-ttu-id="f93ac-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f93ac-139">Int32</span></span>|<span data-ttu-id="f93ac-140">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="f93ac-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="f93ac-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="f93ac-141">acceptedDateTime</span></span>|<span data-ttu-id="f93ac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f93ac-142">DateTimeOffset</span></span>|<span data-ttu-id="f93ac-143">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f93ac-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="f93ac-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f93ac-144">userPrincipalName</span></span>|<span data-ttu-id="f93ac-145">String</span><span class="sxs-lookup"><span data-stu-id="f93ac-145">String</span></span>|<span data-ttu-id="f93ac-146">接受术语的用户的 userPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f93ac-146">The userPrincipalName of the User that accepted the term.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f93ac-147">关系</span><span class="sxs-lookup"><span data-stu-id="f93ac-147">Relationships</span></span>
|<span data-ttu-id="f93ac-148">关系</span><span class="sxs-lookup"><span data-stu-id="f93ac-148">Relationship</span></span>|<span data-ttu-id="f93ac-149">类型</span><span class="sxs-lookup"><span data-stu-id="f93ac-149">Type</span></span>|<span data-ttu-id="f93ac-150">说明</span><span class="sxs-lookup"><span data-stu-id="f93ac-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93ac-151">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f93ac-151">termsAndConditions</span></span>|[<span data-ttu-id="f93ac-152">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f93ac-152">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="f93ac-153">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="f93ac-153">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f93ac-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f93ac-154">JSON Representation</span></span>
<span data-ttu-id="f93ac-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f93ac-155">Here is a JSON representation of the resource.</span></span>
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




