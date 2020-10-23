---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 276a9bd60e988d0bb961ef849c8ce57d8eb9bb47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723951"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="17ee2-103">officeConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="17ee2-103">officeConfiguration resource type</span></span>

<span data-ttu-id="17ee2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17ee2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17ee2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17ee2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17ee2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17ee2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17ee2-107">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="17ee2-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="17ee2-108">Methods</span><span class="sxs-lookup"><span data-stu-id="17ee2-108">Methods</span></span>
|<span data-ttu-id="17ee2-109">方法</span><span class="sxs-lookup"><span data-stu-id="17ee2-109">Method</span></span>|<span data-ttu-id="17ee2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="17ee2-110">Return Type</span></span>|<span data-ttu-id="17ee2-111">说明</span><span class="sxs-lookup"><span data-stu-id="17ee2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ee2-112">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="17ee2-112">Get officeConfiguration</span></span>|[<span data-ttu-id="17ee2-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="17ee2-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="17ee2-114">读取 [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17ee2-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="17ee2-115">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="17ee2-115">Update officeConfiguration</span></span>|[<span data-ttu-id="17ee2-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="17ee2-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="17ee2-117">更新 [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17ee2-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17ee2-118">属性</span><span class="sxs-lookup"><span data-stu-id="17ee2-118">Properties</span></span>
|<span data-ttu-id="17ee2-119">属性</span><span class="sxs-lookup"><span data-stu-id="17ee2-119">Property</span></span>|<span data-ttu-id="17ee2-120">类型</span><span class="sxs-lookup"><span data-stu-id="17ee2-120">Type</span></span>|<span data-ttu-id="17ee2-121">说明</span><span class="sxs-lookup"><span data-stu-id="17ee2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ee2-122">id</span><span class="sxs-lookup"><span data-stu-id="17ee2-122">id</span></span>|<span data-ttu-id="17ee2-123">String</span><span class="sxs-lookup"><span data-stu-id="17ee2-123">String</span></span>|<span data-ttu-id="17ee2-124">Office 配置的 Id。</span><span class="sxs-lookup"><span data-stu-id="17ee2-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="17ee2-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="17ee2-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="17ee2-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17ee2-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="17ee2-127">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="17ee2-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="17ee2-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="17ee2-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="17ee2-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="17ee2-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="17ee2-130">描述租户签入 statues 的实体</span><span class="sxs-lookup"><span data-stu-id="17ee2-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="17ee2-131">关系</span><span class="sxs-lookup"><span data-stu-id="17ee2-131">Relationships</span></span>
|<span data-ttu-id="17ee2-132">关系</span><span class="sxs-lookup"><span data-stu-id="17ee2-132">Relationship</span></span>|<span data-ttu-id="17ee2-133">类型</span><span class="sxs-lookup"><span data-stu-id="17ee2-133">Type</span></span>|<span data-ttu-id="17ee2-134">说明</span><span class="sxs-lookup"><span data-stu-id="17ee2-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ee2-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="17ee2-135">clientConfigurations</span></span>|<span data-ttu-id="17ee2-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17ee2-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="17ee2-137">Office 客户端配置的列表。</span><span class="sxs-lookup"><span data-stu-id="17ee2-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17ee2-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17ee2-138">JSON Representation</span></span>
<span data-ttu-id="17ee2-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17ee2-139">Here is a JSON representation of the resource.</span></span>
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





