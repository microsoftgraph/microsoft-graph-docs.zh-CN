---
title: comanagementEligibleDevicesSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c7244bd594e38a8f129aa81389b159caff6b928
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214636"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a><span data-ttu-id="1486a-103">comanagementEligibleDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1486a-103">comanagementEligibleDevicesSummary resource type</span></span>

<span data-ttu-id="1486a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1486a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1486a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1486a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1486a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1486a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1486a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1486a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1486a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1486a-108">Properties</span></span>
|<span data-ttu-id="1486a-109">属性</span><span class="sxs-lookup"><span data-stu-id="1486a-109">Property</span></span>|<span data-ttu-id="1486a-110">类型</span><span class="sxs-lookup"><span data-stu-id="1486a-110">Type</span></span>|<span data-ttu-id="1486a-111">说明</span><span class="sxs-lookup"><span data-stu-id="1486a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1486a-112">comanagedCount</span><span class="sxs-lookup"><span data-stu-id="1486a-112">comanagedCount</span></span>|<span data-ttu-id="1486a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1486a-113">Int32</span></span>|<span data-ttu-id="1486a-114">已 Co-Managed 的设备计数</span><span class="sxs-lookup"><span data-stu-id="1486a-114">Count of devices already Co-Managed</span></span>|
|<span data-ttu-id="1486a-115">eligibleCount</span><span class="sxs-lookup"><span data-stu-id="1486a-115">eligibleCount</span></span>|<span data-ttu-id="1486a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1486a-116">Int32</span></span>|<span data-ttu-id="1486a-117">完全符合条件的设备计数 Co-Management</span><span class="sxs-lookup"><span data-stu-id="1486a-117">Count of devices fully eligible for Co-Management</span></span>|
|<span data-ttu-id="1486a-118">eligibleButNotAzureAdJoinedCount</span><span class="sxs-lookup"><span data-stu-id="1486a-118">eligibleButNotAzureAdJoinedCount</span></span>|<span data-ttu-id="1486a-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1486a-119">Int32</span></span>|<span data-ttu-id="1486a-120">符合 Co-Management 但尚未加入 Azure Active Directory 的设备的计数</span><span class="sxs-lookup"><span data-stu-id="1486a-120">Count of devices eligible for Co-Management but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="1486a-121">needsOsUpdateCount</span><span class="sxs-lookup"><span data-stu-id="1486a-121">needsOsUpdateCount</span></span>|<span data-ttu-id="1486a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1486a-122">Int32</span></span>|<span data-ttu-id="1486a-123">在 OS 更新后符合 Co-Management 的设备的计数</span><span class="sxs-lookup"><span data-stu-id="1486a-123">Count of devices that will be eligible for Co-Management after an OS update</span></span>|
|<span data-ttu-id="1486a-124">ineligibleCount</span><span class="sxs-lookup"><span data-stu-id="1486a-124">ineligibleCount</span></span>|<span data-ttu-id="1486a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1486a-125">Int32</span></span>|<span data-ttu-id="1486a-126">不符合要求的设备的计数 Co-Management</span><span class="sxs-lookup"><span data-stu-id="1486a-126">Count of devices ineligible for Co-Management</span></span>|

## <a name="relationships"></a><span data-ttu-id="1486a-127">关系</span><span class="sxs-lookup"><span data-stu-id="1486a-127">Relationships</span></span>
<span data-ttu-id="1486a-128">无</span><span class="sxs-lookup"><span data-stu-id="1486a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1486a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1486a-129">JSON Representation</span></span>
<span data-ttu-id="1486a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1486a-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```




