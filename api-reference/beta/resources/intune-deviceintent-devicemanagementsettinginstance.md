---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49f97d47b5ff75e927a5637356476392047a2f8c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807908"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="2cc02-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cc02-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="2cc02-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2cc02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc02-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cc02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc02-106">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="2cc02-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="2cc02-107">方法</span><span class="sxs-lookup"><span data-stu-id="2cc02-107">Methods</span></span>
|<span data-ttu-id="2cc02-108">方法</span><span class="sxs-lookup"><span data-stu-id="2cc02-108">Method</span></span>|<span data-ttu-id="2cc02-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2cc02-109">Return Type</span></span>|<span data-ttu-id="2cc02-110">说明</span><span class="sxs-lookup"><span data-stu-id="2cc02-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2cc02-111">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="2cc02-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="2cc02-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="2cc02-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="2cc02-113">列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cc02-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="2cc02-114">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2cc02-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="2cc02-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2cc02-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="2cc02-116">读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cc02-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2cc02-117">属性</span><span class="sxs-lookup"><span data-stu-id="2cc02-117">Properties</span></span>
|<span data-ttu-id="2cc02-118">属性</span><span class="sxs-lookup"><span data-stu-id="2cc02-118">Property</span></span>|<span data-ttu-id="2cc02-119">类型</span><span class="sxs-lookup"><span data-stu-id="2cc02-119">Type</span></span>|<span data-ttu-id="2cc02-120">说明</span><span class="sxs-lookup"><span data-stu-id="2cc02-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc02-121">id</span><span class="sxs-lookup"><span data-stu-id="2cc02-121">id</span></span>|<span data-ttu-id="2cc02-122">String</span><span class="sxs-lookup"><span data-stu-id="2cc02-122">String</span></span>|<span data-ttu-id="2cc02-123">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="2cc02-123">The setting instance ID</span></span>|
|<span data-ttu-id="2cc02-124">definitionId</span><span class="sxs-lookup"><span data-stu-id="2cc02-124">definitionId</span></span>|<span data-ttu-id="2cc02-125">String</span><span class="sxs-lookup"><span data-stu-id="2cc02-125">String</span></span>|<span data-ttu-id="2cc02-126">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="2cc02-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="2cc02-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="2cc02-127">valueJson</span></span>|<span data-ttu-id="2cc02-128">String</span><span class="sxs-lookup"><span data-stu-id="2cc02-128">String</span></span>|<span data-ttu-id="2cc02-129">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cc02-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc02-130">关系</span><span class="sxs-lookup"><span data-stu-id="2cc02-130">Relationships</span></span>
<span data-ttu-id="2cc02-131">无</span><span class="sxs-lookup"><span data-stu-id="2cc02-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cc02-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cc02-132">JSON Representation</span></span>
<span data-ttu-id="2cc02-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cc02-133">Here is a JSON representation of the resource.</span></span>
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





