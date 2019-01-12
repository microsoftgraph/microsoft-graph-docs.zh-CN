---
title: termsAndConditionsAcceptanceStatus 资源类型
description: C） 由指定用户的策略。 用户必须接受最新版本的条款，才能保留对公司门户的访问权限。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c66b7ba799def675ab3b74ad2ea9b8ce2f7ec22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961076"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="10695-104">termsAndConditionsAcceptanceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="10695-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="10695-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="10695-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10695-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="10695-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10695-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10695-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10695-108">termsAndConditionsAcceptanceStatus 实体表示给定用户对给定条款和条件 (T&C) 策略的接受状态。</span><span class="sxs-lookup"><span data-stu-id="10695-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="10695-109">用户必须接受最新版本的条款，才能保留对公司门户的访问权限。</span><span class="sxs-lookup"><span data-stu-id="10695-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="10695-110">方法</span><span class="sxs-lookup"><span data-stu-id="10695-110">Methods</span></span>
|<span data-ttu-id="10695-111">方法</span><span class="sxs-lookup"><span data-stu-id="10695-111">Method</span></span>|<span data-ttu-id="10695-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="10695-112">Return Type</span></span>|<span data-ttu-id="10695-113">说明</span><span class="sxs-lookup"><span data-stu-id="10695-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10695-114">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="10695-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="10695-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="10695-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="10695-116">列出 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10695-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="10695-117">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="10695-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="10695-119">读取 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10695-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="10695-120">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="10695-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="10695-122">创建新的 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10695-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="10695-123">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="10695-124">无</span><span class="sxs-lookup"><span data-stu-id="10695-124">None</span></span>|<span data-ttu-id="10695-125">删除 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="10695-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="10695-126">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="10695-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="10695-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="10695-128">更新 [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10695-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10695-129">属性</span><span class="sxs-lookup"><span data-stu-id="10695-129">Properties</span></span>
|<span data-ttu-id="10695-130">属性</span><span class="sxs-lookup"><span data-stu-id="10695-130">Property</span></span>|<span data-ttu-id="10695-131">类型</span><span class="sxs-lookup"><span data-stu-id="10695-131">Type</span></span>|<span data-ttu-id="10695-132">说明</span><span class="sxs-lookup"><span data-stu-id="10695-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10695-133">id</span><span class="sxs-lookup"><span data-stu-id="10695-133">id</span></span>|<span data-ttu-id="10695-134">String</span><span class="sxs-lookup"><span data-stu-id="10695-134">String</span></span>|<span data-ttu-id="10695-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="10695-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="10695-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="10695-136">userDisplayName</span></span>|<span data-ttu-id="10695-137">String</span><span class="sxs-lookup"><span data-stu-id="10695-137">String</span></span>|<span data-ttu-id="10695-138">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="10695-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="10695-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="10695-139">acceptedVersion</span></span>|<span data-ttu-id="10695-140">Int32</span><span class="sxs-lookup"><span data-stu-id="10695-140">Int32</span></span>|<span data-ttu-id="10695-141">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="10695-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="10695-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="10695-142">acceptedDateTime</span></span>|<span data-ttu-id="10695-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10695-143">DateTimeOffset</span></span>|<span data-ttu-id="10695-144">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="10695-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10695-145">关系</span><span class="sxs-lookup"><span data-stu-id="10695-145">Relationships</span></span>
|<span data-ttu-id="10695-146">关系</span><span class="sxs-lookup"><span data-stu-id="10695-146">Relationship</span></span>|<span data-ttu-id="10695-147">类型</span><span class="sxs-lookup"><span data-stu-id="10695-147">Type</span></span>|<span data-ttu-id="10695-148">说明</span><span class="sxs-lookup"><span data-stu-id="10695-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10695-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="10695-149">termsAndConditions</span></span>|[<span data-ttu-id="10695-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="10695-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="10695-151">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="10695-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10695-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10695-152">JSON Representation</span></span>
<span data-ttu-id="10695-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10695-153">Here is a JSON representation of the resource.</span></span>
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





