---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9aef844dd4957b75b51f8d16014c2253b0253cc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523607"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="d2831-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2831-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="d2831-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2831-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2831-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2831-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2831-106">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="d2831-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="d2831-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2831-107">Methods</span></span>
|<span data-ttu-id="d2831-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2831-108">Method</span></span>|<span data-ttu-id="d2831-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2831-109">Return Type</span></span>|<span data-ttu-id="d2831-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2831-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2831-111">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="d2831-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="d2831-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="d2831-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="d2831-113">列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2831-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="d2831-114">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d2831-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="d2831-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="d2831-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="d2831-116">读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2831-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2831-117">属性</span><span class="sxs-lookup"><span data-stu-id="d2831-117">Properties</span></span>
|<span data-ttu-id="d2831-118">属性</span><span class="sxs-lookup"><span data-stu-id="d2831-118">Property</span></span>|<span data-ttu-id="d2831-119">类型</span><span class="sxs-lookup"><span data-stu-id="d2831-119">Type</span></span>|<span data-ttu-id="d2831-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2831-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2831-121">id</span><span class="sxs-lookup"><span data-stu-id="d2831-121">id</span></span>|<span data-ttu-id="d2831-122">String</span><span class="sxs-lookup"><span data-stu-id="d2831-122">String</span></span>|<span data-ttu-id="d2831-123">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="d2831-123">The setting instance ID</span></span>|
|<span data-ttu-id="d2831-124">definitionId</span><span class="sxs-lookup"><span data-stu-id="d2831-124">definitionId</span></span>|<span data-ttu-id="d2831-125">String</span><span class="sxs-lookup"><span data-stu-id="d2831-125">String</span></span>|<span data-ttu-id="d2831-126">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="d2831-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="d2831-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="d2831-127">valueJson</span></span>|<span data-ttu-id="d2831-128">String</span><span class="sxs-lookup"><span data-stu-id="d2831-128">String</span></span>|<span data-ttu-id="d2831-129">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2831-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2831-130">关系</span><span class="sxs-lookup"><span data-stu-id="d2831-130">Relationships</span></span>
<span data-ttu-id="d2831-131">无</span><span class="sxs-lookup"><span data-stu-id="d2831-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2831-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2831-132">JSON Representation</span></span>
<span data-ttu-id="d2831-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2831-133">Here is a JSON representation of the resource.</span></span>
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







