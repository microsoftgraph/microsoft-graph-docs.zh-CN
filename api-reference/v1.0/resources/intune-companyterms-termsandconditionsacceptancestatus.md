---
title: termsAndConditionsAcceptanceStatus 资源类型
description: C） 由指定用户的策略。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dffbcf3b13fd988a75e4f1061a52dfc46f193bb5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971373"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="f733c-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f733c-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="f733c-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f733c-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f733c-106">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="f733c-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="f733c-107">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f733c-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="f733c-108">方法</span><span class="sxs-lookup"><span data-stu-id="f733c-108">Methods</span></span>
|<span data-ttu-id="f733c-109">方法</span><span class="sxs-lookup"><span data-stu-id="f733c-109">Method</span></span>|<span data-ttu-id="f733c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f733c-110">Return Type</span></span>|<span data-ttu-id="f733c-111">说明</span><span class="sxs-lookup"><span data-stu-id="f733c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f733c-112">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="f733c-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="f733c-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f733c-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="f733c-114">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f733c-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="f733c-115">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="f733c-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="f733c-117">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f733c-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="f733c-118">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="f733c-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="f733c-120">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f733c-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="f733c-121">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="f733c-122">无</span><span class="sxs-lookup"><span data-stu-id="f733c-122">None</span></span>|<span data-ttu-id="f733c-123">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="f733c-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="f733c-124">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="f733c-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="f733c-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="f733c-126">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f733c-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f733c-127">属性</span><span class="sxs-lookup"><span data-stu-id="f733c-127">Properties</span></span>
|<span data-ttu-id="f733c-128">属性</span><span class="sxs-lookup"><span data-stu-id="f733c-128">Property</span></span>|<span data-ttu-id="f733c-129">类型</span><span class="sxs-lookup"><span data-stu-id="f733c-129">Type</span></span>|<span data-ttu-id="f733c-130">说明</span><span class="sxs-lookup"><span data-stu-id="f733c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f733c-131">id</span><span class="sxs-lookup"><span data-stu-id="f733c-131">id</span></span>|<span data-ttu-id="f733c-132">String</span><span class="sxs-lookup"><span data-stu-id="f733c-132">String</span></span>|<span data-ttu-id="f733c-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f733c-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f733c-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f733c-134">userDisplayName</span></span>|<span data-ttu-id="f733c-135">String</span><span class="sxs-lookup"><span data-stu-id="f733c-135">String</span></span>|<span data-ttu-id="f733c-136">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f733c-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="f733c-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="f733c-137">acceptedVersion</span></span>|<span data-ttu-id="f733c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f733c-138">Int32</span></span>|<span data-ttu-id="f733c-139">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="f733c-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="f733c-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="f733c-140">acceptedDateTime</span></span>|<span data-ttu-id="f733c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f733c-141">DateTimeOffset</span></span>|<span data-ttu-id="f733c-142">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f733c-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f733c-143">关系</span><span class="sxs-lookup"><span data-stu-id="f733c-143">Relationships</span></span>
|<span data-ttu-id="f733c-144">关系</span><span class="sxs-lookup"><span data-stu-id="f733c-144">Relationship</span></span>|<span data-ttu-id="f733c-145">类型</span><span class="sxs-lookup"><span data-stu-id="f733c-145">Type</span></span>|<span data-ttu-id="f733c-146">说明</span><span class="sxs-lookup"><span data-stu-id="f733c-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f733c-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f733c-147">termsAndConditions</span></span>|[<span data-ttu-id="f733c-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f733c-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="f733c-149">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="f733c-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f733c-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f733c-150">JSON Representation</span></span>
<span data-ttu-id="f733c-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f733c-151">Here is a JSON representation of the resource.</span></span>
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



