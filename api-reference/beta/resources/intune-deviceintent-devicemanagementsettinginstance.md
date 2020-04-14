---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaf2cba65c0d6f9cafcce0a4ecef0878a60d1e84
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447191"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="be3be-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="be3be-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="be3be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be3be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be3be-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be3be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be3be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be3be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be3be-107">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="be3be-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="be3be-108">方法</span><span class="sxs-lookup"><span data-stu-id="be3be-108">Methods</span></span>
|<span data-ttu-id="be3be-109">方法</span><span class="sxs-lookup"><span data-stu-id="be3be-109">Method</span></span>|<span data-ttu-id="be3be-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="be3be-110">Return Type</span></span>|<span data-ttu-id="be3be-111">说明</span><span class="sxs-lookup"><span data-stu-id="be3be-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be3be-112">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="be3be-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="be3be-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="be3be-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="be3be-114">列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be3be-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="be3be-115">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="be3be-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="be3be-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="be3be-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="be3be-117">读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be3be-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be3be-118">属性</span><span class="sxs-lookup"><span data-stu-id="be3be-118">Properties</span></span>
|<span data-ttu-id="be3be-119">属性</span><span class="sxs-lookup"><span data-stu-id="be3be-119">Property</span></span>|<span data-ttu-id="be3be-120">类型</span><span class="sxs-lookup"><span data-stu-id="be3be-120">Type</span></span>|<span data-ttu-id="be3be-121">说明</span><span class="sxs-lookup"><span data-stu-id="be3be-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be3be-122">id</span><span class="sxs-lookup"><span data-stu-id="be3be-122">id</span></span>|<span data-ttu-id="be3be-123">String</span><span class="sxs-lookup"><span data-stu-id="be3be-123">String</span></span>|<span data-ttu-id="be3be-124">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="be3be-124">The setting instance ID</span></span>|
|<span data-ttu-id="be3be-125">definitionId</span><span class="sxs-lookup"><span data-stu-id="be3be-125">definitionId</span></span>|<span data-ttu-id="be3be-126">String</span><span class="sxs-lookup"><span data-stu-id="be3be-126">String</span></span>|<span data-ttu-id="be3be-127">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="be3be-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="be3be-128">valueJson</span><span class="sxs-lookup"><span data-stu-id="be3be-128">valueJson</span></span>|<span data-ttu-id="be3be-129">String</span><span class="sxs-lookup"><span data-stu-id="be3be-129">String</span></span>|<span data-ttu-id="be3be-130">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be3be-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="be3be-131">关系</span><span class="sxs-lookup"><span data-stu-id="be3be-131">Relationships</span></span>
<span data-ttu-id="be3be-132">无</span><span class="sxs-lookup"><span data-stu-id="be3be-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be3be-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be3be-133">JSON Representation</span></span>
<span data-ttu-id="be3be-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be3be-134">Here is a JSON representation of the resource.</span></span>
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



