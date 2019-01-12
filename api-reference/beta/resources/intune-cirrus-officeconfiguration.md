---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 767782e26dd203e2ab5488b30520d8cbcf44d1e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921358"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="cc6c5-103">officeConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc6c5-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="cc6c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc6c5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc6c5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc6c5-107">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="cc6c5-108">方法</span><span class="sxs-lookup"><span data-stu-id="cc6c5-108">Methods</span></span>
|<span data-ttu-id="cc6c5-109">方法</span><span class="sxs-lookup"><span data-stu-id="cc6c5-109">Method</span></span>|<span data-ttu-id="cc6c5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc6c5-110">Return Type</span></span>|<span data-ttu-id="cc6c5-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc6c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc6c5-112">获取 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc6c5-112">Get officeConfiguration</span></span>|[<span data-ttu-id="cc6c5-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc6c5-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="cc6c5-114">读取属性和[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="cc6c5-115">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc6c5-115">Update officeConfiguration</span></span>|[<span data-ttu-id="cc6c5-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc6c5-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="cc6c5-117">更新[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc6c5-118">属性</span><span class="sxs-lookup"><span data-stu-id="cc6c5-118">Properties</span></span>
|<span data-ttu-id="cc6c5-119">属性</span><span class="sxs-lookup"><span data-stu-id="cc6c5-119">Property</span></span>|<span data-ttu-id="cc6c5-120">类型</span><span class="sxs-lookup"><span data-stu-id="cc6c5-120">Type</span></span>|<span data-ttu-id="cc6c5-121">说明</span><span class="sxs-lookup"><span data-stu-id="cc6c5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc6c5-122">id</span><span class="sxs-lookup"><span data-stu-id="cc6c5-122">id</span></span>|<span data-ttu-id="cc6c5-123">字符串</span><span class="sxs-lookup"><span data-stu-id="cc6c5-123">String</span></span>|<span data-ttu-id="cc6c5-124">Office 配置的 id。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="cc6c5-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="cc6c5-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="cc6c5-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc6c5-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="cc6c5-127">Office 客户端中签入状态的列表。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="cc6c5-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="cc6c5-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="cc6c5-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="cc6c5-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="cc6c5-130">介绍租户中签入状态使用的实体</span><span class="sxs-lookup"><span data-stu-id="cc6c5-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc6c5-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="cc6c5-131">Relationships</span></span>
|<span data-ttu-id="cc6c5-132">关系</span><span class="sxs-lookup"><span data-stu-id="cc6c5-132">Relationship</span></span>|<span data-ttu-id="cc6c5-133">类型</span><span class="sxs-lookup"><span data-stu-id="cc6c5-133">Type</span></span>|<span data-ttu-id="cc6c5-134">说明</span><span class="sxs-lookup"><span data-stu-id="cc6c5-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc6c5-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="cc6c5-135">clientConfigurations</span></span>|<span data-ttu-id="cc6c5-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc6c5-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="cc6c5-137">Office 客户端配置的列表。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc6c5-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc6c5-138">JSON Representation</span></span>
<span data-ttu-id="cc6c5-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc6c5-139">Here is a JSON representation of the resource.</span></span>
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



