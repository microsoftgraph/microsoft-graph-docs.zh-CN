---
title: comanagementEligibleDevicesSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b67734bf98a48c31a1346bd730c8521fd8a8d681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060767"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a><span data-ttu-id="79ae7-103">comanagementEligibleDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="79ae7-103">comanagementEligibleDevicesSummary resource type</span></span>

<span data-ttu-id="79ae7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79ae7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79ae7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79ae7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79ae7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ae7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="79ae7-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="79ae7-108">属性</span><span class="sxs-lookup"><span data-stu-id="79ae7-108">Properties</span></span>
|<span data-ttu-id="79ae7-109">属性</span><span class="sxs-lookup"><span data-stu-id="79ae7-109">Property</span></span>|<span data-ttu-id="79ae7-110">类型</span><span class="sxs-lookup"><span data-stu-id="79ae7-110">Type</span></span>|<span data-ttu-id="79ae7-111">说明</span><span class="sxs-lookup"><span data-stu-id="79ae7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ae7-112">comanagedCount</span><span class="sxs-lookup"><span data-stu-id="79ae7-112">comanagedCount</span></span>|<span data-ttu-id="79ae7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="79ae7-113">Int32</span></span>|<span data-ttu-id="79ae7-114">已进行共同管理的设备的计数</span><span class="sxs-lookup"><span data-stu-id="79ae7-114">Count of devices already Co-Managed</span></span>|
|<span data-ttu-id="79ae7-115">eligibleCount</span><span class="sxs-lookup"><span data-stu-id="79ae7-115">eligibleCount</span></span>|<span data-ttu-id="79ae7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="79ae7-116">Int32</span></span>|<span data-ttu-id="79ae7-117">完全符合共同管理条件的设备的数量</span><span class="sxs-lookup"><span data-stu-id="79ae7-117">Count of devices fully eligible for Co-Management</span></span>|
|<span data-ttu-id="79ae7-118">eligibleButNotAzureAdJoinedCount</span><span class="sxs-lookup"><span data-stu-id="79ae7-118">eligibleButNotAzureAdJoinedCount</span></span>|<span data-ttu-id="79ae7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="79ae7-119">Int32</span></span>|<span data-ttu-id="79ae7-120">符合共同管理但尚未加入 Azure Active Directory 的设备的计数</span><span class="sxs-lookup"><span data-stu-id="79ae7-120">Count of devices eligible for Co-Management but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="79ae7-121">needsOsUpdateCount</span><span class="sxs-lookup"><span data-stu-id="79ae7-121">needsOsUpdateCount</span></span>|<span data-ttu-id="79ae7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="79ae7-122">Int32</span></span>|<span data-ttu-id="79ae7-123">在 OS 更新之后符合共同管理条件的设备的计数</span><span class="sxs-lookup"><span data-stu-id="79ae7-123">Count of devices that will be eligible for Co-Management after an OS update</span></span>|
|<span data-ttu-id="79ae7-124">ineligibleCount</span><span class="sxs-lookup"><span data-stu-id="79ae7-124">ineligibleCount</span></span>|<span data-ttu-id="79ae7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="79ae7-125">Int32</span></span>|<span data-ttu-id="79ae7-126">不符合共同管理要求的设备的计数</span><span class="sxs-lookup"><span data-stu-id="79ae7-126">Count of devices ineligible for Co-Management</span></span>|

## <a name="relationships"></a><span data-ttu-id="79ae7-127">关系</span><span class="sxs-lookup"><span data-stu-id="79ae7-127">Relationships</span></span>
<span data-ttu-id="79ae7-128">无</span><span class="sxs-lookup"><span data-stu-id="79ae7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79ae7-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79ae7-129">JSON Representation</span></span>
<span data-ttu-id="79ae7-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79ae7-130">Here is a JSON representation of the resource.</span></span>
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






