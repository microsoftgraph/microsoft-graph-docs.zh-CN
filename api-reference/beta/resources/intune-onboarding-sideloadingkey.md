---
title: sideLoadingKey 资源类型
description: Windows 8 和租户 8.1 设备安装业务线应用程序需要 SideLoadingKey 实体。
author: tfitzmac
ms.openlocfilehash: 66dc833ab46f8dc1c030a3ef97be78cd73ee3660
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304310"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="dc995-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc995-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="dc995-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dc995-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc995-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dc995-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc995-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dc995-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc995-107">Windows 8 和租户 8.1 设备安装业务线应用程序需要 SideLoadingKey 实体。</span><span class="sxs-lookup"><span data-stu-id="dc995-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="dc995-108">方法</span><span class="sxs-lookup"><span data-stu-id="dc995-108">Methods</span></span>
|<span data-ttu-id="dc995-109">方法</span><span class="sxs-lookup"><span data-stu-id="dc995-109">Method</span></span>|<span data-ttu-id="dc995-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc995-110">Return Type</span></span>|<span data-ttu-id="dc995-111">说明</span><span class="sxs-lookup"><span data-stu-id="dc995-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc995-112">列表 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="dc995-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="dc995-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="dc995-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="dc995-114">列出属性和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="dc995-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="dc995-115">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="dc995-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="dc995-117">读取属性和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="dc995-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="dc995-118">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="dc995-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="dc995-120">创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dc995-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="dc995-121">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="dc995-122">无</span><span class="sxs-lookup"><span data-stu-id="dc995-122">None</span></span>|<span data-ttu-id="dc995-123">删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="dc995-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="dc995-124">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="dc995-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="dc995-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="dc995-126">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc995-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc995-127">属性</span><span class="sxs-lookup"><span data-stu-id="dc995-127">Properties</span></span>
|<span data-ttu-id="dc995-128">属性</span><span class="sxs-lookup"><span data-stu-id="dc995-128">Property</span></span>|<span data-ttu-id="dc995-129">类型</span><span class="sxs-lookup"><span data-stu-id="dc995-129">Type</span></span>|<span data-ttu-id="dc995-130">说明</span><span class="sxs-lookup"><span data-stu-id="dc995-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc995-131">id</span><span class="sxs-lookup"><span data-stu-id="dc995-131">id</span></span>|<span data-ttu-id="dc995-132">字符串</span><span class="sxs-lookup"><span data-stu-id="dc995-132">String</span></span>|<span data-ttu-id="dc995-133">端加载关键的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="dc995-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="dc995-134">值</span><span class="sxs-lookup"><span data-stu-id="dc995-134">value</span></span>|<span data-ttu-id="dc995-135">字符串</span><span class="sxs-lookup"><span data-stu-id="dc995-135">String</span></span>|<span data-ttu-id="dc995-136">端加载密钥值是 5x5 的值，通过 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="dc995-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="dc995-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dc995-137">displayName</span></span>|<span data-ttu-id="dc995-138">字符串</span><span class="sxs-lookup"><span data-stu-id="dc995-138">String</span></span>|<span data-ttu-id="dc995-139">端加载项显示名称为 it 专业人员管理员。</span><span class="sxs-lookup"><span data-stu-id="dc995-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="dc995-140">说明</span><span class="sxs-lookup"><span data-stu-id="dc995-140">description</span></span>|<span data-ttu-id="dc995-141">字符串</span><span class="sxs-lookup"><span data-stu-id="dc995-141">String</span></span>|<span data-ttu-id="dc995-142">显示为 it 专业人员 Admins 端加载项说明正在</span><span class="sxs-lookup"><span data-stu-id="dc995-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="dc995-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="dc995-143">totalActivation</span></span>|<span data-ttu-id="dc995-144">Int32</span><span class="sxs-lookup"><span data-stu-id="dc995-144">Int32</span></span>|<span data-ttu-id="dc995-145">端加载项总激活向 it 专业人员 Admins 显示。</span><span class="sxs-lookup"><span data-stu-id="dc995-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="dc995-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc995-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="dc995-147">字符串</span><span class="sxs-lookup"><span data-stu-id="dc995-147">String</span></span>|<span data-ttu-id="dc995-148">端加载项上次更新日期向 it 专业人员 Admins 显示。</span><span class="sxs-lookup"><span data-stu-id="dc995-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc995-149">Relationships</span><span class="sxs-lookup"><span data-stu-id="dc995-149">Relationships</span></span>
<span data-ttu-id="dc995-150">无</span><span class="sxs-lookup"><span data-stu-id="dc995-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc995-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc995-151">JSON Representation</span></span>
<span data-ttu-id="dc995-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc995-152">Here is a JSON representation of the resource.</span></span>
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





