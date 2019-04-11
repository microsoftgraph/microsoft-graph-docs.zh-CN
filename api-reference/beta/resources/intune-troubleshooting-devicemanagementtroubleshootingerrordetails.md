---
title: deviceManagementTroubleshootingErrorDetails 资源类型
description: 包含有关错误及其修正的详细信息的对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cfcbe0688836fa394237f1a25656540e401555f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796183"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="d9a0e-103">deviceManagementTroubleshootingErrorDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9a0e-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="d9a0e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9a0e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a0e-106">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="d9a0e-107">属性</span><span class="sxs-lookup"><span data-stu-id="d9a0e-107">Properties</span></span>
|<span data-ttu-id="d9a0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9a0e-108">Property</span></span>|<span data-ttu-id="d9a0e-109">类型</span><span class="sxs-lookup"><span data-stu-id="d9a0e-109">Type</span></span>|<span data-ttu-id="d9a0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="d9a0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a0e-111">context</span><span class="sxs-lookup"><span data-stu-id="d9a0e-111">context</span></span>|<span data-ttu-id="d9a0e-112">String</span><span class="sxs-lookup"><span data-stu-id="d9a0e-112">String</span></span>|<span data-ttu-id="d9a0e-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9a0e-113">Not yet documented</span></span>|
|<span data-ttu-id="d9a0e-114">出</span><span class="sxs-lookup"><span data-stu-id="d9a0e-114">failure</span></span>|<span data-ttu-id="d9a0e-115">String</span><span class="sxs-lookup"><span data-stu-id="d9a0e-115">String</span></span>|<span data-ttu-id="d9a0e-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9a0e-116">Not yet documented</span></span>|
|<span data-ttu-id="d9a0e-117">failureDetails</span><span class="sxs-lookup"><span data-stu-id="d9a0e-117">failureDetails</span></span>|<span data-ttu-id="d9a0e-118">String</span><span class="sxs-lookup"><span data-stu-id="d9a0e-118">String</span></span>|<span data-ttu-id="d9a0e-119">出现问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="d9a0e-120">纠正</span><span class="sxs-lookup"><span data-stu-id="d9a0e-120">remediation</span></span>|<span data-ttu-id="d9a0e-121">String</span><span class="sxs-lookup"><span data-stu-id="d9a0e-121">String</span></span>|<span data-ttu-id="d9a0e-122">有关如何修正此问题的详细说明。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="d9a0e-123">资源</span><span class="sxs-lookup"><span data-stu-id="d9a0e-123">resources</span></span>|<span data-ttu-id="d9a0e-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9a0e-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="d9a0e-125">指向有关此故障的有用文档的链接。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9a0e-126">关系</span><span class="sxs-lookup"><span data-stu-id="d9a0e-126">Relationships</span></span>
<span data-ttu-id="d9a0e-127">无</span><span class="sxs-lookup"><span data-stu-id="d9a0e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9a0e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9a0e-128">JSON Representation</span></span>
<span data-ttu-id="d9a0e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9a0e-129">Here is a JSON representation of the resource.</span></span>
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



