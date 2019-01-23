---
title: sideLoadingKey 资源类型
description: Windows 8 和租户 8.1 设备安装业务线应用程序需要 SideLoadingKey 实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f7be853faae78e0ac7528d0127fd11b928164ee9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410040"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="a788c-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="a788c-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="a788c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a788c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a788c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a788c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a788c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a788c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a788c-107">Windows 8 和租户 8.1 设备安装业务线应用程序需要 SideLoadingKey 实体。</span><span class="sxs-lookup"><span data-stu-id="a788c-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="a788c-108">方法</span><span class="sxs-lookup"><span data-stu-id="a788c-108">Methods</span></span>
|<span data-ttu-id="a788c-109">方法</span><span class="sxs-lookup"><span data-stu-id="a788c-109">Method</span></span>|<span data-ttu-id="a788c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a788c-110">Return Type</span></span>|<span data-ttu-id="a788c-111">说明</span><span class="sxs-lookup"><span data-stu-id="a788c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a788c-112">列表 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="a788c-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="a788c-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="a788c-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="a788c-114">列出属性和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="a788c-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="a788c-115">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="a788c-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="a788c-117">读取属性和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a788c-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="a788c-118">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="a788c-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="a788c-120">创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a788c-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="a788c-121">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="a788c-122">无</span><span class="sxs-lookup"><span data-stu-id="a788c-122">None</span></span>|<span data-ttu-id="a788c-123">删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="a788c-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="a788c-124">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="a788c-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="a788c-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="a788c-126">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a788c-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a788c-127">属性</span><span class="sxs-lookup"><span data-stu-id="a788c-127">Properties</span></span>
|<span data-ttu-id="a788c-128">属性</span><span class="sxs-lookup"><span data-stu-id="a788c-128">Property</span></span>|<span data-ttu-id="a788c-129">类型</span><span class="sxs-lookup"><span data-stu-id="a788c-129">Type</span></span>|<span data-ttu-id="a788c-130">说明</span><span class="sxs-lookup"><span data-stu-id="a788c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a788c-131">id</span><span class="sxs-lookup"><span data-stu-id="a788c-131">id</span></span>|<span data-ttu-id="a788c-132">String</span><span class="sxs-lookup"><span data-stu-id="a788c-132">String</span></span>|<span data-ttu-id="a788c-133">端加载关键的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="a788c-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="a788c-134">值</span><span class="sxs-lookup"><span data-stu-id="a788c-134">value</span></span>|<span data-ttu-id="a788c-135">String</span><span class="sxs-lookup"><span data-stu-id="a788c-135">String</span></span>|<span data-ttu-id="a788c-136">端加载密钥值是 5x5 的值，通过 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="a788c-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="a788c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a788c-137">displayName</span></span>|<span data-ttu-id="a788c-138">String</span><span class="sxs-lookup"><span data-stu-id="a788c-138">String</span></span>|<span data-ttu-id="a788c-139">端加载项显示名称为 it 专业人员管理员。</span><span class="sxs-lookup"><span data-stu-id="a788c-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="a788c-140">说明</span><span class="sxs-lookup"><span data-stu-id="a788c-140">description</span></span>|<span data-ttu-id="a788c-141">String</span><span class="sxs-lookup"><span data-stu-id="a788c-141">String</span></span>|<span data-ttu-id="a788c-142">显示为 it 专业人员 Admins 端加载项说明正在</span><span class="sxs-lookup"><span data-stu-id="a788c-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="a788c-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="a788c-143">totalActivation</span></span>|<span data-ttu-id="a788c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a788c-144">Int32</span></span>|<span data-ttu-id="a788c-145">端加载项总激活向 it 专业人员 Admins 显示。</span><span class="sxs-lookup"><span data-stu-id="a788c-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="a788c-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a788c-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="a788c-147">String</span><span class="sxs-lookup"><span data-stu-id="a788c-147">String</span></span>|<span data-ttu-id="a788c-148">端加载项上次更新日期向 it 专业人员 Admins 显示。</span><span class="sxs-lookup"><span data-stu-id="a788c-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a788c-149">关系</span><span class="sxs-lookup"><span data-stu-id="a788c-149">Relationships</span></span>
<span data-ttu-id="a788c-150">无</span><span class="sxs-lookup"><span data-stu-id="a788c-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a788c-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a788c-151">JSON Representation</span></span>
<span data-ttu-id="a788c-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a788c-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```




