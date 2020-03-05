---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6967972cbc94d28d6fde605ba72f3497b9b48e46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488241"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="d3c90-103">officeConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3c90-103">officeConfiguration resource type</span></span>

<span data-ttu-id="d3c90-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d3c90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3c90-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3c90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3c90-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3c90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c90-107">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="d3c90-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="d3c90-108">方法</span><span class="sxs-lookup"><span data-stu-id="d3c90-108">Methods</span></span>
|<span data-ttu-id="d3c90-109">方法</span><span class="sxs-lookup"><span data-stu-id="d3c90-109">Method</span></span>|<span data-ttu-id="d3c90-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3c90-110">Return Type</span></span>|<span data-ttu-id="d3c90-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3c90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c90-112">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3c90-112">Get officeConfiguration</span></span>|[<span data-ttu-id="d3c90-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3c90-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="d3c90-114">读取[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3c90-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="d3c90-115">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3c90-115">Update officeConfiguration</span></span>|[<span data-ttu-id="d3c90-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3c90-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="d3c90-117">更新[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3c90-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3c90-118">属性</span><span class="sxs-lookup"><span data-stu-id="d3c90-118">Properties</span></span>
|<span data-ttu-id="d3c90-119">属性</span><span class="sxs-lookup"><span data-stu-id="d3c90-119">Property</span></span>|<span data-ttu-id="d3c90-120">类型</span><span class="sxs-lookup"><span data-stu-id="d3c90-120">Type</span></span>|<span data-ttu-id="d3c90-121">说明</span><span class="sxs-lookup"><span data-stu-id="d3c90-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c90-122">id</span><span class="sxs-lookup"><span data-stu-id="d3c90-122">id</span></span>|<span data-ttu-id="d3c90-123">String</span><span class="sxs-lookup"><span data-stu-id="d3c90-123">String</span></span>|<span data-ttu-id="d3c90-124">Office 配置的 Id。</span><span class="sxs-lookup"><span data-stu-id="d3c90-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="d3c90-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="d3c90-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="d3c90-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3c90-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="d3c90-127">Office 客户端签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="d3c90-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="d3c90-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d3c90-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="d3c90-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d3c90-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="d3c90-130">描述租户签入 statues 的实体</span><span class="sxs-lookup"><span data-stu-id="d3c90-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3c90-131">关系</span><span class="sxs-lookup"><span data-stu-id="d3c90-131">Relationships</span></span>
|<span data-ttu-id="d3c90-132">关系</span><span class="sxs-lookup"><span data-stu-id="d3c90-132">Relationship</span></span>|<span data-ttu-id="d3c90-133">类型</span><span class="sxs-lookup"><span data-stu-id="d3c90-133">Type</span></span>|<span data-ttu-id="d3c90-134">说明</span><span class="sxs-lookup"><span data-stu-id="d3c90-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c90-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="d3c90-135">clientConfigurations</span></span>|<span data-ttu-id="d3c90-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3c90-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="d3c90-137">Office 客户端配置的列表。</span><span class="sxs-lookup"><span data-stu-id="d3c90-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3c90-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3c90-138">JSON Representation</span></span>
<span data-ttu-id="d3c90-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3c90-139">Here is a JSON representation of the resource.</span></span>
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



