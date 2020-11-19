---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 包含有关错误及其修正的详细信息的对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e28d47e9ab8752c733a32bb96f2685bfd90bd6d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255334"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="25d00-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="25d00-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

<span data-ttu-id="25d00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25d00-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25d00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25d00-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25d00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25d00-107">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="25d00-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="25d00-108">属性</span><span class="sxs-lookup"><span data-stu-id="25d00-108">Properties</span></span>
|<span data-ttu-id="25d00-109">属性</span><span class="sxs-lookup"><span data-stu-id="25d00-109">Property</span></span>|<span data-ttu-id="25d00-110">类型</span><span class="sxs-lookup"><span data-stu-id="25d00-110">Type</span></span>|<span data-ttu-id="25d00-111">描述</span><span class="sxs-lookup"><span data-stu-id="25d00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d00-112">context</span><span class="sxs-lookup"><span data-stu-id="25d00-112">context</span></span>|<span data-ttu-id="25d00-113">String</span><span class="sxs-lookup"><span data-stu-id="25d00-113">String</span></span>|<span data-ttu-id="25d00-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25d00-114">Not yet documented</span></span>|
|<span data-ttu-id="25d00-115">出</span><span class="sxs-lookup"><span data-stu-id="25d00-115">failure</span></span>|<span data-ttu-id="25d00-116">String</span><span class="sxs-lookup"><span data-stu-id="25d00-116">String</span></span>|<span data-ttu-id="25d00-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25d00-117">Not yet documented</span></span>|
|<span data-ttu-id="25d00-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="25d00-118">failureDetails</span></span>|<span data-ttu-id="25d00-119">String</span><span class="sxs-lookup"><span data-stu-id="25d00-119">String</span></span>|<span data-ttu-id="25d00-120">出现问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="25d00-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="25d00-121">纠正</span><span class="sxs-lookup"><span data-stu-id="25d00-121">remediation</span></span>|<span data-ttu-id="25d00-122">String</span><span class="sxs-lookup"><span data-stu-id="25d00-122">String</span></span>|<span data-ttu-id="25d00-123">有关如何修正此问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="25d00-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="25d00-124">resources</span><span class="sxs-lookup"><span data-stu-id="25d00-124">resources</span></span>|<span data-ttu-id="25d00-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25d00-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="25d00-126">指向有关此故障的有用文档的链接。</span><span class="sxs-lookup"><span data-stu-id="25d00-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25d00-127">关系</span><span class="sxs-lookup"><span data-stu-id="25d00-127">Relationships</span></span>
<span data-ttu-id="25d00-128">无</span><span class="sxs-lookup"><span data-stu-id="25d00-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25d00-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25d00-129">JSON Representation</span></span>
<span data-ttu-id="25d00-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25d00-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




