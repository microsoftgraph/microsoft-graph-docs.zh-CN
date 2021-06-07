---
title: deviceAppManagement 资源类型
description: 充当所有设备应用管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b99cd14d949d4043fe1ecb4b911c6f89a8f12b10
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756413"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="a142f-103">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a142f-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="a142f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a142f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a142f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a142f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a142f-106">充当所有设备应用管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="a142f-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="a142f-107">方法</span><span class="sxs-lookup"><span data-stu-id="a142f-107">Methods</span></span>
|<span data-ttu-id="a142f-108">方法</span><span class="sxs-lookup"><span data-stu-id="a142f-108">Method</span></span>|<span data-ttu-id="a142f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a142f-109">Return Type</span></span>|<span data-ttu-id="a142f-110">说明</span><span class="sxs-lookup"><span data-stu-id="a142f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a142f-111">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a142f-111">Get deviceAppManagement</span></span>](../api/intune-apps-deviceappmanagement-get.md)|[<span data-ttu-id="a142f-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a142f-112">deviceAppManagement</span></span>](../resources/intune-apps-deviceappmanagement.md)|<span data-ttu-id="a142f-113">读取 [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a142f-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="a142f-114">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a142f-114">Update deviceAppManagement</span></span>](../api/intune-apps-deviceappmanagement-update.md)|[<span data-ttu-id="a142f-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="a142f-115">deviceAppManagement</span></span>](../resources/intune-apps-deviceappmanagement.md)|<span data-ttu-id="a142f-116">更新 [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a142f-116">Update the properties of a [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a142f-117">属性</span><span class="sxs-lookup"><span data-stu-id="a142f-117">Properties</span></span>
|<span data-ttu-id="a142f-118">属性</span><span class="sxs-lookup"><span data-stu-id="a142f-118">Property</span></span>|<span data-ttu-id="a142f-119">类型</span><span class="sxs-lookup"><span data-stu-id="a142f-119">Type</span></span>|<span data-ttu-id="a142f-120">说明</span><span class="sxs-lookup"><span data-stu-id="a142f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a142f-121">id</span><span class="sxs-lookup"><span data-stu-id="a142f-121">id</span></span>|<span data-ttu-id="a142f-122">String</span><span class="sxs-lookup"><span data-stu-id="a142f-122">String</span></span>|<span data-ttu-id="a142f-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a142f-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a142f-124">关系</span><span class="sxs-lookup"><span data-stu-id="a142f-124">Relationships</span></span>
|<span data-ttu-id="a142f-125">关系</span><span class="sxs-lookup"><span data-stu-id="a142f-125">Relationship</span></span>|<span data-ttu-id="a142f-126">类型</span><span class="sxs-lookup"><span data-stu-id="a142f-126">Type</span></span>|<span data-ttu-id="a142f-127">说明</span><span class="sxs-lookup"><span data-stu-id="a142f-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a142f-128">mobileApps</span><span class="sxs-lookup"><span data-stu-id="a142f-128">mobileApps</span></span>|<span data-ttu-id="a142f-129">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a142f-129">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="a142f-130">移动应用。</span><span class="sxs-lookup"><span data-stu-id="a142f-130">The mobile apps.</span></span>|
|<span data-ttu-id="a142f-131">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="a142f-131">mobileAppCategories</span></span>|<span data-ttu-id="a142f-132">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a142f-132">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="a142f-133">移动应用类别。</span><span class="sxs-lookup"><span data-stu-id="a142f-133">The mobile app categories.</span></span>|
|<span data-ttu-id="a142f-134">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="a142f-134">mobileAppConfigurations</span></span>|<span data-ttu-id="a142f-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a142f-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="a142f-136">托管设备移动应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="a142f-136">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a142f-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a142f-137">JSON Representation</span></span>
<span data-ttu-id="a142f-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a142f-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




