---
title: groupPolicyOperation 资源类型
description: 实体表示组策略操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69ab3503d761052ba8293b9133f43204a6afd7b0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376915"
---
# <a name="grouppolicyoperation-resource-type"></a><span data-ttu-id="b8e1e-103">groupPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8e1e-103">groupPolicyOperation resource type</span></span>

<span data-ttu-id="b8e1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8e1e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8e1e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e1e-107">实体表示组策略操作。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-107">The entity represents an group policy operation.</span></span>

## <a name="methods"></a><span data-ttu-id="b8e1e-108">方法</span><span class="sxs-lookup"><span data-stu-id="b8e1e-108">Methods</span></span>
|<span data-ttu-id="b8e1e-109">方法</span><span class="sxs-lookup"><span data-stu-id="b8e1e-109">Method</span></span>|<span data-ttu-id="b8e1e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8e1e-110">Return Type</span></span>|<span data-ttu-id="b8e1e-111">说明</span><span class="sxs-lookup"><span data-stu-id="b8e1e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8e1e-112">列出 groupPolicyOperations</span><span class="sxs-lookup"><span data-stu-id="b8e1e-112">List groupPolicyOperations</span></span>](../api/intune-grouppolicy-grouppolicyoperation-list.md)|<span data-ttu-id="b8e1e-113">[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="b8e1e-113">[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) collection</span></span>|<span data-ttu-id="b8e1e-114">列出[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-114">List properties and relationships of the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) objects.</span></span>|
|[<span data-ttu-id="b8e1e-115">获取 groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-115">Get groupPolicyOperation</span></span>](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[<span data-ttu-id="b8e1e-116">groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-116">groupPolicyOperation</span></span>](../resources/intune-grouppolicy-grouppolicyoperation.md)|<span data-ttu-id="b8e1e-117">读取[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-117">Read properties and relationships of the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>|
|[<span data-ttu-id="b8e1e-118">创建 groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-118">Create groupPolicyOperation</span></span>](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[<span data-ttu-id="b8e1e-119">groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-119">groupPolicyOperation</span></span>](../resources/intune-grouppolicy-grouppolicyoperation.md)|<span data-ttu-id="b8e1e-120">创建新的[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-120">Create a new [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>|
|[<span data-ttu-id="b8e1e-121">删除 groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-121">Delete groupPolicyOperation</span></span>](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|<span data-ttu-id="b8e1e-122">无</span><span class="sxs-lookup"><span data-stu-id="b8e1e-122">None</span></span>|<span data-ttu-id="b8e1e-123">删除[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-123">Deletes a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span></span>|
|[<span data-ttu-id="b8e1e-124">更新 groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-124">Update groupPolicyOperation</span></span>](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[<span data-ttu-id="b8e1e-125">groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="b8e1e-125">groupPolicyOperation</span></span>](../resources/intune-grouppolicy-grouppolicyoperation.md)|<span data-ttu-id="b8e1e-126">更新[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-126">Update the properties of a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8e1e-127">属性</span><span class="sxs-lookup"><span data-stu-id="b8e1e-127">Properties</span></span>
|<span data-ttu-id="b8e1e-128">属性</span><span class="sxs-lookup"><span data-stu-id="b8e1e-128">Property</span></span>|<span data-ttu-id="b8e1e-129">类型</span><span class="sxs-lookup"><span data-stu-id="b8e1e-129">Type</span></span>|<span data-ttu-id="b8e1e-130">说明</span><span class="sxs-lookup"><span data-stu-id="b8e1e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e1e-131">operationType</span><span class="sxs-lookup"><span data-stu-id="b8e1e-131">operationType</span></span>|[<span data-ttu-id="b8e1e-132">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="b8e1e-132">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="b8e1e-133">组策略操作的类型。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-133">The type of group policy operation.</span></span> <span data-ttu-id="b8e1e-134">可取值为：`none`、`upload`、`uploadNewVersion`、`addLanguageFiles`、`removeLanguageFiles`、`updateLanguageFiles` 或 `remove`。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-134">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="b8e1e-135">operationStatus</span><span class="sxs-lookup"><span data-stu-id="b8e1e-135">operationStatus</span></span>|[<span data-ttu-id="b8e1e-136">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="b8e1e-136">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="b8e1e-137">组策略操作状态。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-137">The group policy operation status.</span></span> <span data-ttu-id="b8e1e-138">可取值为：`unknown`、`inProgress`、`success`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-138">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="b8e1e-139">statusDetails</span><span class="sxs-lookup"><span data-stu-id="b8e1e-139">statusDetails</span></span>|<span data-ttu-id="b8e1e-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b8e1e-140">String</span></span>|<span data-ttu-id="b8e1e-141">组策略操作状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-141">The group policy operation status detail.</span></span>|
|<span data-ttu-id="b8e1e-142">id</span><span class="sxs-lookup"><span data-stu-id="b8e1e-142">id</span></span>|<span data-ttu-id="b8e1e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b8e1e-143">String</span></span>|<span data-ttu-id="b8e1e-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-144">Key of the entity.</span></span>|
|<span data-ttu-id="b8e1e-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8e1e-145">lastModifiedDateTime</span></span>|<span data-ttu-id="b8e1e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8e1e-146">DateTimeOffset</span></span>|<span data-ttu-id="b8e1e-147">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e1e-148">关系</span><span class="sxs-lookup"><span data-stu-id="b8e1e-148">Relationships</span></span>
<span data-ttu-id="b8e1e-149">无</span><span class="sxs-lookup"><span data-stu-id="b8e1e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8e1e-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8e1e-150">JSON Representation</span></span>
<span data-ttu-id="b8e1e-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8e1e-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



