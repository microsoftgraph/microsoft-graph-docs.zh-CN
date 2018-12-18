---
title: managedMobileApp 资源类型
description: 部署应用的标识符。
author: tfitzmac
ms.openlocfilehash: f6cb1c74ef46bd08de695d1447c2b88cfeaee187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308790"
---
# <a name="managedmobileapp-resource-type"></a><span data-ttu-id="d5c3a-103">managedMobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5c3a-103">managedMobileApp resource type</span></span>

> <span data-ttu-id="d5c3a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5c3a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c3a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5c3a-107">部署应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-107">The identifier for the deployment an app.</span></span>
## <a name="methods"></a><span data-ttu-id="d5c3a-108">方法</span><span class="sxs-lookup"><span data-stu-id="d5c3a-108">Methods</span></span>
|<span data-ttu-id="d5c3a-109">方法</span><span class="sxs-lookup"><span data-stu-id="d5c3a-109">Method</span></span>|<span data-ttu-id="d5c3a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5c3a-110">Return Type</span></span>|<span data-ttu-id="d5c3a-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5c3a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5c3a-112">列出 managedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d5c3a-112">List managedMobileApps</span></span>](../api/intune-mam-managedmobileapp-list.md)|<span data-ttu-id="d5c3a-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5c3a-113">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="d5c3a-114">列出 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-114">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>|
|[<span data-ttu-id="d5c3a-115">获取 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-115">Get managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-get.md)|[<span data-ttu-id="d5c3a-116">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-116">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="d5c3a-117">读取 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-117">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="d5c3a-118">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-118">Create managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-create.md)|[<span data-ttu-id="d5c3a-119">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-119">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="d5c3a-120">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-120">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|
|[<span data-ttu-id="d5c3a-121">删除 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-121">Delete managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-delete.md)|<span data-ttu-id="d5c3a-122">无</span><span class="sxs-lookup"><span data-stu-id="d5c3a-122">None</span></span>|<span data-ttu-id="d5c3a-123">删除 [managedMobileApp](../resources/intune-mam-managedmobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-123">Deletes a [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>|
|[<span data-ttu-id="d5c3a-124">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-124">Update managedMobileApp</span></span>](../api/intune-mam-managedmobileapp-update.md)|[<span data-ttu-id="d5c3a-125">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d5c3a-125">managedMobileApp</span></span>](../resources/intune-mam-managedmobileapp.md)|<span data-ttu-id="d5c3a-126">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-126">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5c3a-127">属性</span><span class="sxs-lookup"><span data-stu-id="d5c3a-127">Properties</span></span>
|<span data-ttu-id="d5c3a-128">属性</span><span class="sxs-lookup"><span data-stu-id="d5c3a-128">Property</span></span>|<span data-ttu-id="d5c3a-129">类型</span><span class="sxs-lookup"><span data-stu-id="d5c3a-129">Type</span></span>|<span data-ttu-id="d5c3a-130">说明</span><span class="sxs-lookup"><span data-stu-id="d5c3a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c3a-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5c3a-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="d5c3a-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5c3a-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d5c3a-133">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d5c3a-134">id</span><span class="sxs-lookup"><span data-stu-id="d5c3a-134">id</span></span>|<span data-ttu-id="d5c3a-135">String</span><span class="sxs-lookup"><span data-stu-id="d5c3a-135">String</span></span>|<span data-ttu-id="d5c3a-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-136">Key of the entity.</span></span>|
|<span data-ttu-id="d5c3a-137">version</span><span class="sxs-lookup"><span data-stu-id="d5c3a-137">version</span></span>|<span data-ttu-id="d5c3a-138">String</span><span class="sxs-lookup"><span data-stu-id="d5c3a-138">String</span></span>|<span data-ttu-id="d5c3a-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-139">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5c3a-140">关系</span><span class="sxs-lookup"><span data-stu-id="d5c3a-140">Relationships</span></span>
<span data-ttu-id="d5c3a-141">无</span><span class="sxs-lookup"><span data-stu-id="d5c3a-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5c3a-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5c3a-142">JSON Representation</span></span>
<span data-ttu-id="d5c3a-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5c3a-143">Here is a JSON representation of the resource.</span></span>
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





