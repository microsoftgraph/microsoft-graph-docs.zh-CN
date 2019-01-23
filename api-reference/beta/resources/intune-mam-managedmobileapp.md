---
title: managedMobileApp 资源类型
description: 部署应用的标识符。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b8de88976937a967f60a0842eeb9f24b465e50f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419252"
---
# <a name="managedmobileapp-resource-type"></a><span data-ttu-id="e08e5-103">managedMobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e08e5-103">managedMobileApp resource type</span></span>

> <span data-ttu-id="e08e5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e08e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e08e5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e08e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e08e5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e08e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e08e5-107">部署应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="e08e5-107">The identifier for the deployment an app.</span></span>

## <a name="methods"></a><span data-ttu-id="e08e5-108">方法</span><span class="sxs-lookup"><span data-stu-id="e08e5-108">Methods</span></span>
|<span data-ttu-id="e08e5-109">方法</span><span class="sxs-lookup"><span data-stu-id="e08e5-109">Method</span></span>|<span data-ttu-id="e08e5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e08e5-110">Return Type</span></span>|<span data-ttu-id="e08e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e08e5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e08e5-112">列出 managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="e08e5-112">List managedMobileApps</span></span>](../api/intune-mam-managedmobileapp-list.md)|<span data-ttu-id="e08e5-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e08e5-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="e08e5-114">列出 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e08e5-114">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>|
|[<span data-ttu-id="e08e5-115">获取 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-115">Get managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-get.md)|[<span data-ttu-id="e08e5-116">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-116">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="e08e5-117">读取 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e08e5-117">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="e08e5-118">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-118">Create managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-create.md)|[<span data-ttu-id="e08e5-119">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-119">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="e08e5-120">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e08e5-120">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="e08e5-121">删除 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-121">Delete managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-delete.md)|<span data-ttu-id="e08e5-122">无</span><span class="sxs-lookup"><span data-stu-id="e08e5-122">None</span></span>|<span data-ttu-id="e08e5-123">删除 [managedMobileApp](../resources/intune-mam-managedmobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e08e5-123">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>|
|[<span data-ttu-id="e08e5-124">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-124">Update managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-update.md)|[<span data-ttu-id="e08e5-125">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="e08e5-125">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="e08e5-126">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e08e5-126">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e08e5-127">属性</span><span class="sxs-lookup"><span data-stu-id="e08e5-127">Properties</span></span>
|<span data-ttu-id="e08e5-128">属性</span><span class="sxs-lookup"><span data-stu-id="e08e5-128">Property</span></span>|<span data-ttu-id="e08e5-129">类型</span><span class="sxs-lookup"><span data-stu-id="e08e5-129">Type</span></span>|<span data-ttu-id="e08e5-130">说明</span><span class="sxs-lookup"><span data-stu-id="e08e5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e08e5-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e08e5-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="e08e5-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e08e5-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e08e5-133">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="e08e5-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="e08e5-134">id</span><span class="sxs-lookup"><span data-stu-id="e08e5-134">id</span></span>|<span data-ttu-id="e08e5-135">String</span><span class="sxs-lookup"><span data-stu-id="e08e5-135">String</span></span>|<span data-ttu-id="e08e5-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e08e5-136">Key of the entity.</span></span>|
|<span data-ttu-id="e08e5-137">version</span><span class="sxs-lookup"><span data-stu-id="e08e5-137">version</span></span>|<span data-ttu-id="e08e5-138">String</span><span class="sxs-lookup"><span data-stu-id="e08e5-138">String</span></span>|<span data-ttu-id="e08e5-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="e08e5-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e08e5-140">关系</span><span class="sxs-lookup"><span data-stu-id="e08e5-140">Relationships</span></span>
<span data-ttu-id="e08e5-141">无</span><span class="sxs-lookup"><span data-stu-id="e08e5-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e08e5-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e08e5-142">JSON Representation</span></span>
<span data-ttu-id="e08e5-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e08e5-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




