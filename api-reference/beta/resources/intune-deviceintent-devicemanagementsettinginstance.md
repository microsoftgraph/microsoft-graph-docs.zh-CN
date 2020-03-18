---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e374faf132e5da0ee3e2213e61fcdcc3078b3300
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785314"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="eef51-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="eef51-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="eef51-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eef51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eef51-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eef51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eef51-106">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="eef51-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="eef51-107">方法</span><span class="sxs-lookup"><span data-stu-id="eef51-107">Methods</span></span>
|<span data-ttu-id="eef51-108">方法</span><span class="sxs-lookup"><span data-stu-id="eef51-108">Method</span></span>|<span data-ttu-id="eef51-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="eef51-109">Return Type</span></span>|<span data-ttu-id="eef51-110">说明</span><span class="sxs-lookup"><span data-stu-id="eef51-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eef51-111">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="eef51-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="eef51-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="eef51-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="eef51-113">列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eef51-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="eef51-114">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="eef51-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="eef51-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="eef51-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="eef51-116">读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eef51-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eef51-117">属性</span><span class="sxs-lookup"><span data-stu-id="eef51-117">Properties</span></span>
|<span data-ttu-id="eef51-118">属性</span><span class="sxs-lookup"><span data-stu-id="eef51-118">Property</span></span>|<span data-ttu-id="eef51-119">类型</span><span class="sxs-lookup"><span data-stu-id="eef51-119">Type</span></span>|<span data-ttu-id="eef51-120">说明</span><span class="sxs-lookup"><span data-stu-id="eef51-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef51-121">id</span><span class="sxs-lookup"><span data-stu-id="eef51-121">id</span></span>|<span data-ttu-id="eef51-122">String</span><span class="sxs-lookup"><span data-stu-id="eef51-122">String</span></span>|<span data-ttu-id="eef51-123">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="eef51-123">The setting instance ID</span></span>|
|<span data-ttu-id="eef51-124">definitionId</span><span class="sxs-lookup"><span data-stu-id="eef51-124">definitionId</span></span>|<span data-ttu-id="eef51-125">String</span><span class="sxs-lookup"><span data-stu-id="eef51-125">String</span></span>|<span data-ttu-id="eef51-126">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="eef51-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="eef51-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="eef51-127">valueJson</span></span>|<span data-ttu-id="eef51-128">String</span><span class="sxs-lookup"><span data-stu-id="eef51-128">String</span></span>|<span data-ttu-id="eef51-129">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eef51-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="eef51-130">关系</span><span class="sxs-lookup"><span data-stu-id="eef51-130">Relationships</span></span>
<span data-ttu-id="eef51-131">无</span><span class="sxs-lookup"><span data-stu-id="eef51-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eef51-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eef51-132">JSON Representation</span></span>
<span data-ttu-id="eef51-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eef51-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



