---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47ee6458d8c045ff99ce244a43e3058d040093fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011972"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="27d40-103">officeConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="27d40-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="27d40-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27d40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27d40-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27d40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27d40-106">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="27d40-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="27d40-107">方法</span><span class="sxs-lookup"><span data-stu-id="27d40-107">Methods</span></span>
|<span data-ttu-id="27d40-108">方法</span><span class="sxs-lookup"><span data-stu-id="27d40-108">Method</span></span>|<span data-ttu-id="27d40-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="27d40-109">Return Type</span></span>|<span data-ttu-id="27d40-110">说明</span><span class="sxs-lookup"><span data-stu-id="27d40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27d40-111">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="27d40-111">Get officeConfiguration</span></span>|[<span data-ttu-id="27d40-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="27d40-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="27d40-113">读取[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27d40-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="27d40-114">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="27d40-114">Update officeConfiguration</span></span>|[<span data-ttu-id="27d40-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="27d40-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="27d40-116">更新[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27d40-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27d40-117">属性</span><span class="sxs-lookup"><span data-stu-id="27d40-117">Properties</span></span>
|<span data-ttu-id="27d40-118">属性</span><span class="sxs-lookup"><span data-stu-id="27d40-118">Property</span></span>|<span data-ttu-id="27d40-119">类型</span><span class="sxs-lookup"><span data-stu-id="27d40-119">Type</span></span>|<span data-ttu-id="27d40-120">说明</span><span class="sxs-lookup"><span data-stu-id="27d40-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27d40-121">id</span><span class="sxs-lookup"><span data-stu-id="27d40-121">id</span></span>|<span data-ttu-id="27d40-122">String</span><span class="sxs-lookup"><span data-stu-id="27d40-122">String</span></span>|<span data-ttu-id="27d40-123">Office 配置的 Id。</span><span class="sxs-lookup"><span data-stu-id="27d40-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="27d40-124">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="27d40-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="27d40-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="27d40-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="27d40-126">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="27d40-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="27d40-127">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="27d40-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="27d40-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="27d40-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="27d40-129">描述租户签入 statues 的实体</span><span class="sxs-lookup"><span data-stu-id="27d40-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="27d40-130">关系</span><span class="sxs-lookup"><span data-stu-id="27d40-130">Relationships</span></span>
|<span data-ttu-id="27d40-131">关系</span><span class="sxs-lookup"><span data-stu-id="27d40-131">Relationship</span></span>|<span data-ttu-id="27d40-132">类型</span><span class="sxs-lookup"><span data-stu-id="27d40-132">Type</span></span>|<span data-ttu-id="27d40-133">说明</span><span class="sxs-lookup"><span data-stu-id="27d40-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27d40-134">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="27d40-134">clientConfigurations</span></span>|<span data-ttu-id="27d40-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="27d40-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="27d40-136">Office 客户端配置的列表。</span><span class="sxs-lookup"><span data-stu-id="27d40-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27d40-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27d40-137">JSON Representation</span></span>
<span data-ttu-id="27d40-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27d40-138">Here is a JSON representation of the resource.</span></span>
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



