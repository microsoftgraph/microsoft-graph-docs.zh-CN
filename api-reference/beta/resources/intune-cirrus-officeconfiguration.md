---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc76295b21602328689ee48f8aed8be74bd82093
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406547"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="feb97-103">officeConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="feb97-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="feb97-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="feb97-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="feb97-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="feb97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="feb97-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="feb97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb97-107">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="feb97-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="feb97-108">方法</span><span class="sxs-lookup"><span data-stu-id="feb97-108">Methods</span></span>
|<span data-ttu-id="feb97-109">方法</span><span class="sxs-lookup"><span data-stu-id="feb97-109">Method</span></span>|<span data-ttu-id="feb97-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="feb97-110">Return Type</span></span>|<span data-ttu-id="feb97-111">说明</span><span class="sxs-lookup"><span data-stu-id="feb97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb97-112">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="feb97-112">Get officeConfiguration</span></span>|[<span data-ttu-id="feb97-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="feb97-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="feb97-114">读取属性和[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="feb97-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="feb97-115">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="feb97-115">Update officeConfiguration</span></span>|[<span data-ttu-id="feb97-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="feb97-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="feb97-117">更新[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="feb97-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="feb97-118">属性</span><span class="sxs-lookup"><span data-stu-id="feb97-118">Properties</span></span>
|<span data-ttu-id="feb97-119">属性</span><span class="sxs-lookup"><span data-stu-id="feb97-119">Property</span></span>|<span data-ttu-id="feb97-120">类型</span><span class="sxs-lookup"><span data-stu-id="feb97-120">Type</span></span>|<span data-ttu-id="feb97-121">说明</span><span class="sxs-lookup"><span data-stu-id="feb97-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb97-122">id</span><span class="sxs-lookup"><span data-stu-id="feb97-122">id</span></span>|<span data-ttu-id="feb97-123">String</span><span class="sxs-lookup"><span data-stu-id="feb97-123">String</span></span>|<span data-ttu-id="feb97-124">Office 配置的 id。</span><span class="sxs-lookup"><span data-stu-id="feb97-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="feb97-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="feb97-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="feb97-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="feb97-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="feb97-127">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="feb97-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="feb97-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="feb97-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="feb97-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="feb97-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="feb97-130">介绍租户中签入状态使用的实体</span><span class="sxs-lookup"><span data-stu-id="feb97-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="feb97-131">关系</span><span class="sxs-lookup"><span data-stu-id="feb97-131">Relationships</span></span>
|<span data-ttu-id="feb97-132">关系</span><span class="sxs-lookup"><span data-stu-id="feb97-132">Relationship</span></span>|<span data-ttu-id="feb97-133">类型</span><span class="sxs-lookup"><span data-stu-id="feb97-133">Type</span></span>|<span data-ttu-id="feb97-134">说明</span><span class="sxs-lookup"><span data-stu-id="feb97-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb97-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="feb97-135">clientConfigurations</span></span>|<span data-ttu-id="feb97-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="feb97-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="feb97-137">Office 客户端配置的列表。</span><span class="sxs-lookup"><span data-stu-id="feb97-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="feb97-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="feb97-138">JSON Representation</span></span>
<span data-ttu-id="feb97-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="feb97-139">Here is a JSON representation of the resource.</span></span>
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



