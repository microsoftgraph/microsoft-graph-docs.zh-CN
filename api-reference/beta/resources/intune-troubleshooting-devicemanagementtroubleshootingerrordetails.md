---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 包含有关错误及其修正的详细信息的对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8f1d6152a51f034d1dbce15b0b7f0113e682bc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087647"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="332d8-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="332d8-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

<span data-ttu-id="332d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="332d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="332d8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="332d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="332d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="332d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="332d8-107">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="332d8-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="332d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="332d8-108">Properties</span></span>
|<span data-ttu-id="332d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="332d8-109">Property</span></span>|<span data-ttu-id="332d8-110">类型</span><span class="sxs-lookup"><span data-stu-id="332d8-110">Type</span></span>|<span data-ttu-id="332d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="332d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="332d8-112">context</span><span class="sxs-lookup"><span data-stu-id="332d8-112">context</span></span>|<span data-ttu-id="332d8-113">String</span><span class="sxs-lookup"><span data-stu-id="332d8-113">String</span></span>|<span data-ttu-id="332d8-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="332d8-114">Not yet documented</span></span>|
|<span data-ttu-id="332d8-115">出</span><span class="sxs-lookup"><span data-stu-id="332d8-115">failure</span></span>|<span data-ttu-id="332d8-116">String</span><span class="sxs-lookup"><span data-stu-id="332d8-116">String</span></span>|<span data-ttu-id="332d8-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="332d8-117">Not yet documented</span></span>|
|<span data-ttu-id="332d8-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="332d8-118">failureDetails</span></span>|<span data-ttu-id="332d8-119">字符串</span><span class="sxs-lookup"><span data-stu-id="332d8-119">String</span></span>|<span data-ttu-id="332d8-120">出现问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="332d8-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="332d8-121">纠正</span><span class="sxs-lookup"><span data-stu-id="332d8-121">remediation</span></span>|<span data-ttu-id="332d8-122">字符串</span><span class="sxs-lookup"><span data-stu-id="332d8-122">String</span></span>|<span data-ttu-id="332d8-123">有关如何修正此问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="332d8-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="332d8-124">resources</span><span class="sxs-lookup"><span data-stu-id="332d8-124">resources</span></span>|<span data-ttu-id="332d8-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="332d8-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="332d8-126">指向有关此故障的有用文档的链接。</span><span class="sxs-lookup"><span data-stu-id="332d8-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="332d8-127">关系</span><span class="sxs-lookup"><span data-stu-id="332d8-127">Relationships</span></span>
<span data-ttu-id="332d8-128">无</span><span class="sxs-lookup"><span data-stu-id="332d8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="332d8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="332d8-129">JSON Representation</span></span>
<span data-ttu-id="332d8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="332d8-130">Here is a JSON representation of the resource.</span></span>
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






