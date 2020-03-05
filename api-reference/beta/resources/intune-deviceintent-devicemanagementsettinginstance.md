---
title: deviceManagementSettingInstance 资源类型
description: 设置实例的基本类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f52c90a7e03ceb2463be3589e60694251d002c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525241"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="c73a9-103">deviceManagementSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="c73a9-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="c73a9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c73a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c73a9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c73a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c73a9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c73a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c73a9-107">设置实例的基本类型</span><span class="sxs-lookup"><span data-stu-id="c73a9-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="c73a9-108">方法</span><span class="sxs-lookup"><span data-stu-id="c73a9-108">Methods</span></span>
|<span data-ttu-id="c73a9-109">方法</span><span class="sxs-lookup"><span data-stu-id="c73a9-109">Method</span></span>|<span data-ttu-id="c73a9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c73a9-110">Return Type</span></span>|<span data-ttu-id="c73a9-111">说明</span><span class="sxs-lookup"><span data-stu-id="c73a9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c73a9-112">列出 deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="c73a9-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="c73a9-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="c73a9-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="c73a9-114">列出[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c73a9-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="c73a9-115">获取 deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c73a9-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="c73a9-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c73a9-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="c73a9-117">读取[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c73a9-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c73a9-118">属性</span><span class="sxs-lookup"><span data-stu-id="c73a9-118">Properties</span></span>
|<span data-ttu-id="c73a9-119">属性</span><span class="sxs-lookup"><span data-stu-id="c73a9-119">Property</span></span>|<span data-ttu-id="c73a9-120">类型</span><span class="sxs-lookup"><span data-stu-id="c73a9-120">Type</span></span>|<span data-ttu-id="c73a9-121">说明</span><span class="sxs-lookup"><span data-stu-id="c73a9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c73a9-122">id</span><span class="sxs-lookup"><span data-stu-id="c73a9-122">id</span></span>|<span data-ttu-id="c73a9-123">String</span><span class="sxs-lookup"><span data-stu-id="c73a9-123">String</span></span>|<span data-ttu-id="c73a9-124">设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="c73a9-124">The setting instance ID</span></span>|
|<span data-ttu-id="c73a9-125">definitionId</span><span class="sxs-lookup"><span data-stu-id="c73a9-125">definitionId</span></span>|<span data-ttu-id="c73a9-126">String</span><span class="sxs-lookup"><span data-stu-id="c73a9-126">String</span></span>|<span data-ttu-id="c73a9-127">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="c73a9-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="c73a9-128">valueJson</span><span class="sxs-lookup"><span data-stu-id="c73a9-128">valueJson</span></span>|<span data-ttu-id="c73a9-129">String</span><span class="sxs-lookup"><span data-stu-id="c73a9-129">String</span></span>|<span data-ttu-id="c73a9-130">值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c73a9-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="c73a9-131">关系</span><span class="sxs-lookup"><span data-stu-id="c73a9-131">Relationships</span></span>
<span data-ttu-id="c73a9-132">无</span><span class="sxs-lookup"><span data-stu-id="c73a9-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c73a9-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c73a9-133">JSON Representation</span></span>
<span data-ttu-id="c73a9-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c73a9-134">Here is a JSON representation of the resource.</span></span>
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



