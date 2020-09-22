---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a035fcb23b3137bfe4e278e12d71a754d1e69d05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061180"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="14507-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="14507-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="14507-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14507-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14507-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14507-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14507-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14507-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14507-107">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="14507-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="14507-108">方法</span><span class="sxs-lookup"><span data-stu-id="14507-108">Methods</span></span>
|<span data-ttu-id="14507-109">方法</span><span class="sxs-lookup"><span data-stu-id="14507-109">Method</span></span>|<span data-ttu-id="14507-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="14507-110">Return Type</span></span>|<span data-ttu-id="14507-111">说明</span><span class="sxs-lookup"><span data-stu-id="14507-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14507-112">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="14507-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="14507-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14507-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="14507-114">列出 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14507-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="14507-115">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="14507-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="14507-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="14507-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="14507-117">读取 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14507-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14507-118">属性</span><span class="sxs-lookup"><span data-stu-id="14507-118">Properties</span></span>
|<span data-ttu-id="14507-119">属性</span><span class="sxs-lookup"><span data-stu-id="14507-119">Property</span></span>|<span data-ttu-id="14507-120">类型</span><span class="sxs-lookup"><span data-stu-id="14507-120">Type</span></span>|<span data-ttu-id="14507-121">说明</span><span class="sxs-lookup"><span data-stu-id="14507-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14507-122">id</span><span class="sxs-lookup"><span data-stu-id="14507-122">id</span></span>|<span data-ttu-id="14507-123">String</span><span class="sxs-lookup"><span data-stu-id="14507-123">String</span></span>|<span data-ttu-id="14507-124">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="14507-124">The setting instance ID</span></span>|
|<span data-ttu-id="14507-125">definitionId</span><span class="sxs-lookup"><span data-stu-id="14507-125">definitionId</span></span>|<span data-ttu-id="14507-126">String</span><span class="sxs-lookup"><span data-stu-id="14507-126">String</span></span>|<span data-ttu-id="14507-127">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="14507-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="14507-128">valueJson</span><span class="sxs-lookup"><span data-stu-id="14507-128">valueJson</span></span>|<span data-ttu-id="14507-129">String</span><span class="sxs-lookup"><span data-stu-id="14507-129">String</span></span>|<span data-ttu-id="14507-130">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14507-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="14507-131">关系</span><span class="sxs-lookup"><span data-stu-id="14507-131">Relationships</span></span>
<span data-ttu-id="14507-132">无</span><span class="sxs-lookup"><span data-stu-id="14507-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14507-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14507-133">JSON Representation</span></span>
<span data-ttu-id="14507-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14507-134">Here is a JSON representation of the resource.</span></span>
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






