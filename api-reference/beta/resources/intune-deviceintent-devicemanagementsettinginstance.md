---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28f380bc2aef749079676d4f97fd4bd6f3d7c671
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364647"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="f7d39-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7d39-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="f7d39-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7d39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7d39-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7d39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d39-106">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="f7d39-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="f7d39-107">方法</span><span class="sxs-lookup"><span data-stu-id="f7d39-107">Methods</span></span>
|<span data-ttu-id="f7d39-108">方法</span><span class="sxs-lookup"><span data-stu-id="f7d39-108">Method</span></span>|<span data-ttu-id="f7d39-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7d39-109">Return Type</span></span>|<span data-ttu-id="f7d39-110">说明</span><span class="sxs-lookup"><span data-stu-id="f7d39-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7d39-111">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="f7d39-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="f7d39-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="f7d39-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="f7d39-113">列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7d39-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="f7d39-114">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f7d39-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="f7d39-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f7d39-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="f7d39-116">读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7d39-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7d39-117">属性</span><span class="sxs-lookup"><span data-stu-id="f7d39-117">Properties</span></span>
|<span data-ttu-id="f7d39-118">属性</span><span class="sxs-lookup"><span data-stu-id="f7d39-118">Property</span></span>|<span data-ttu-id="f7d39-119">类型</span><span class="sxs-lookup"><span data-stu-id="f7d39-119">Type</span></span>|<span data-ttu-id="f7d39-120">说明</span><span class="sxs-lookup"><span data-stu-id="f7d39-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d39-121">id</span><span class="sxs-lookup"><span data-stu-id="f7d39-121">id</span></span>|<span data-ttu-id="f7d39-122">String</span><span class="sxs-lookup"><span data-stu-id="f7d39-122">String</span></span>|<span data-ttu-id="f7d39-123">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="f7d39-123">The setting instance ID</span></span>|
|<span data-ttu-id="f7d39-124">definitionId</span><span class="sxs-lookup"><span data-stu-id="f7d39-124">definitionId</span></span>|<span data-ttu-id="f7d39-125">String</span><span class="sxs-lookup"><span data-stu-id="f7d39-125">String</span></span>|<span data-ttu-id="f7d39-126">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="f7d39-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="f7d39-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="f7d39-127">valueJson</span></span>|<span data-ttu-id="f7d39-128">String</span><span class="sxs-lookup"><span data-stu-id="f7d39-128">String</span></span>|<span data-ttu-id="f7d39-129">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7d39-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d39-130">关系</span><span class="sxs-lookup"><span data-stu-id="f7d39-130">Relationships</span></span>
<span data-ttu-id="f7d39-131">无</span><span class="sxs-lookup"><span data-stu-id="f7d39-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7d39-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7d39-132">JSON Representation</span></span>
<span data-ttu-id="f7d39-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7d39-133">Here is a JSON representation of the resource.</span></span>
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



