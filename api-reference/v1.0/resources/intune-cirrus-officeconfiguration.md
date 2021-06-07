---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20e86afa8d0d5fddf5b87a6c6667e2e16baa391a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752891"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="0b1a8-103">officeConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b1a8-103">officeConfiguration resource type</span></span>

<span data-ttu-id="0b1a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b1a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b1a8-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b1a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b1a8-107">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="0b1a8-108">方法</span><span class="sxs-lookup"><span data-stu-id="0b1a8-108">Methods</span></span>
|<span data-ttu-id="0b1a8-109">方法</span><span class="sxs-lookup"><span data-stu-id="0b1a8-109">Method</span></span>|<span data-ttu-id="0b1a8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b1a8-110">Return Type</span></span>|<span data-ttu-id="0b1a8-111">说明</span><span class="sxs-lookup"><span data-stu-id="0b1a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b1a8-112">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b1a8-112">Get officeConfiguration</span></span>|[<span data-ttu-id="0b1a8-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b1a8-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="0b1a8-114">读取 [officeConfiguration 对象的属性和](../resources/intune-cirrus-officeconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="0b1a8-115">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b1a8-115">Update officeConfiguration</span></span>|[<span data-ttu-id="0b1a8-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b1a8-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="0b1a8-117">更新 [officeConfiguration 对象](../resources/intune-cirrus-officeconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b1a8-118">属性</span><span class="sxs-lookup"><span data-stu-id="0b1a8-118">Properties</span></span>
|<span data-ttu-id="0b1a8-119">属性</span><span class="sxs-lookup"><span data-stu-id="0b1a8-119">Property</span></span>|<span data-ttu-id="0b1a8-120">类型</span><span class="sxs-lookup"><span data-stu-id="0b1a8-120">Type</span></span>|<span data-ttu-id="0b1a8-121">说明</span><span class="sxs-lookup"><span data-stu-id="0b1a8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b1a8-122">id</span><span class="sxs-lookup"><span data-stu-id="0b1a8-122">id</span></span>|<span data-ttu-id="0b1a8-123">String</span><span class="sxs-lookup"><span data-stu-id="0b1a8-123">String</span></span>|<span data-ttu-id="0b1a8-124">Office 配置的 ID。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="0b1a8-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="0b1a8-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="0b1a8-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b1a8-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="0b1a8-127">Office 客户端签入状态列表。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="0b1a8-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0b1a8-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="0b1a8-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0b1a8-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="0b1a8-130">描述租户签入计划的实体</span><span class="sxs-lookup"><span data-stu-id="0b1a8-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b1a8-131">关系</span><span class="sxs-lookup"><span data-stu-id="0b1a8-131">Relationships</span></span>
|<span data-ttu-id="0b1a8-132">关系</span><span class="sxs-lookup"><span data-stu-id="0b1a8-132">Relationship</span></span>|<span data-ttu-id="0b1a8-133">类型</span><span class="sxs-lookup"><span data-stu-id="0b1a8-133">Type</span></span>|<span data-ttu-id="0b1a8-134">说明</span><span class="sxs-lookup"><span data-stu-id="0b1a8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b1a8-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="0b1a8-135">clientConfigurations</span></span>|<span data-ttu-id="0b1a8-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b1a8-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="0b1a8-137">Office 客户端配置列表。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b1a8-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b1a8-138">JSON Representation</span></span>
<span data-ttu-id="0b1a8-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b1a8-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```




